<template>
  <section id="open-source" class="open-source">
    <div class="open-source_wrap">
      <div class="container">
        <h2 class="sec-title">{{$t('Besides the main work, our teams contribute to open source')}}</h2>
        <ButtonLinkBlack :data="{text: $t('btn-link--black'), icon: 'github-light.svg', link: 'https://github.com/maddevsio'}" />
      </div>
    </div>
    <div class="open-source_wrap-projects">
      <h2 class="sec-title">{{$t('Projects')}}<span class="our-pets">🐶 🐱</span></h2>
      <div class="open-source_wrap-projects_list">
        <a href="https://gps.maddevs.io/ru/" target="_blank" rel="noreferrer" class="open-source_wrap-projects_list-item op-proj-1">
          <div class="projects-img_wrap">
            <img src="../../assets/img/Home/svg/openSource/mlm.svg" alt="Mad Location Manager">
          </div>
          <div class="projects-desc_wrap">
            <h4>Mad Location Manager</h4>
            <p>{{$t("Accurate and ”pure” data from GPS-recivers proceeded with Kalman's filter")}}</p>
          </div>
        </a>
        <a href="https://heimdall.maddevs.io" target="_blank" rel="noreferrer" class="open-source_wrap-projects_list-item op-proj-2">
          <div class="projects-img_wrap">
            <img src="../../assets/img/Home/svg/openSource/Heimdall.svg" class="op-img-sf" alt="Heimdall">
          </div>
          <div class="projects-desc_wrap">
            <h4>Heimdall</h4>
            <p>{{$t('Tool for monitoring the security of Ethereum smart contracts as a badge in the repository')}}</p>
          </div>
        </a>
        <a href="https://comedian.maddevs.io" target="_blank" rel="noreferrer" class="open-source_wrap-projects_list-item op-proj-3">
          <div class="projects-img_wrap">
            <img src="../../assets/img/Home/svg/openSource/comedian.svg" class="op-img-sf" alt="Comedian">
          </div>
          <div class="projects-desc_wrap">
            <h4>Comedian</h4>
            <p>{{$t('pet-projects_item-desc-3')}}</p>
          </div>
        </a>
        <a href="https://idmatch.co" target="_blank" rel="noreferrer" class="open-source_wrap-projects_list-item op-proj-4">
          <div class="projects-img_wrap">
            <img src="../../assets/img/Home/svg/openSource/id.svg" class="op-img-opensourse" alt="IDmatch">
          </div>
          <div class="projects-desc_wrap">
            <h4>IDmatch</h4>
            <p>{{$t('Artifical Intelligence and machine learning for personal identification')}}</p>
          </div>
        </a>
        <div class="open-source_wrap-projects_list-hidden_blocks" :class="{ show_proj: showProj }">
          <a href="https://github.com/maddevsio/madpwa" target="_blank" rel="noreferrer" class="open-source_wrap-projects_list-item op-proj-5">
            <div class="projects-img_wrap">
              <img src="../../assets/img/Home/svg/openSource/madpwa.svg" class="op-img-madpwa" alt="MadPwa">
            </div>
            <div class="projects-desc_wrap">
              <h4>MADPWA</h4>
              <p>{{$t('Set of libraries for the quick, convinient and easy way creation of PWA')}}</p>
            </div>
          </a>
          <a href="https://github.com/maddevsio/ariadna" target="_blank" rel="noreferrer" class="open-source_wrap-projects_list-item op-proj-6">
            <div class="projects-img_wrap">
              <img src="../../assets/img/Home/svg/openSource/ariadna.svg" alt="Mad Location Manager">
            </div>
            <div class="projects-desc_wrap">
              <h4>Ariadna</h4>
              <p>{{$t('The open-source geocoder built on top of ElasticSearch for fast geocoding')}}</p>
            </div>
          </a>
          <a href="https://blog.maddevs.io/https-blog-maddevs-io-yourcast-tv-32915159be1c" target="_blank" rel="noreferrer" class="open-source_wrap-projects_list-item op-proj-7">
            <div class="projects-img_wrap">
              <img src="../../assets/img/Home/svg/openSource/yourcast.svg" alt="MadPwa">
            </div>
            <div class="projects-desc_wrap">
              <h4>Yourcast</h4>
              <p>{{$t('Bot that forms the video playlist and transfers the data to HLS stream in browser')}}</p>
            </div>
          </a>
        </div>
      </div>
    </div>
    <div class="open-source_btn" @click="toggleAllProj()">
      <span v-if="!showProj">
        {{ $t('I want more open source projects') }}
        <img src="../../assets/img/Home/svg/openSource/right.svg" alt="Show more">
      </span>
      <a href="https://github.com/maddevsio" target="_blank" rel="noreferrer" v-else>
        {{ $t('View all projects on GitHub') }}
        <img src="../../assets/img/Home/svg/openSource/right.svg" alt="Show more">
      </a>
    </div>
  </section>
</template>

<script>
import ButtonLinkBlack from '../blocks/button-link--black';

export default {
  name: 'open-source',
  data() {
    return {
      showProj: false,
      githubData: {
        repos: 0,
        commits: 0,
        stars: 0,
        forks: 0,
        updated_at: 0,
        tasks: 0
      },
    };
  },
  components: {
    ButtonLinkBlack
  },
  methods: {
    toggleAllProj() {
      this.showProj = true;
    }
  },
};
</script>
