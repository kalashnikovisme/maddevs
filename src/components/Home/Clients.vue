<template>
  <section id="clients" class="clients">
    <div class="container">
      <div class="clients_wrap" :class="{ open_wrap: OpenWrap }">
        <h2 class="sec-title">{{$t('Our clients')}}</h2>
        <div class="clients_wrap-icons">
          <div class="clients_wrap-icons_row">
            <a class="small-image">
              <img src="../../assets/img/Home/svg/clients/veeqo.svg" alt="veeqo">
            </a>
            <a class="small-image">
              <img src="../../assets/img/Home/svg/clients/nappy.svg" alt="nappy">
            </a>
            <a>
              <img src="../../assets/img/Home/svg/clients/eatigo.svg" alt="eatigo">
            </a>
            <a class="small-image">
              <img src="../../assets/img/Home/svg/clients/triggermesh.svg" alt="triggermesh">
            </a>
            <a>
              <img src="../../assets/img/Home/svg/clients/kickico.svg" alt="kickico">
            </a>
            <a class="small-image">
              <img src="../../assets/img/Home/svg/clients/teacherly.svg" alt="teacherly">
            </a>
            <a>
              <img src="../../assets/img/Home/svg/clients/localize.svg" alt="localize">
            </a>
            <a>
              <img src="../../assets/img/Home/svg/clients/terbine.svg" alt="terbine">
            </a>
            <a>
              <img src="../../assets/img/Home/svg/clients/zentist.svg" alt="zentist">
            </a>
            <a>
              <img src="../../assets/img/Home/svg/clients/admitad.svg" alt="admitad">
            </a>
            <a class="small-image">
              <img src="../../assets/img/Home/svg/clients/nuntiux.svg" alt="nuntiux">
            </a>
            <a>
              <img src="../../assets/img/Home/svg/clients/namba.svg" alt="namba">
            </a>
            <a>
              <img src="../../assets/img/Home/svg/clients/zofice.svg" alt="zofice">
            </a>
            <a>
              <img src="../../assets/img/Home/svg/clients/iotsploit.svg" alt="iotsploit">
            </a>
            <a>
              <img src="../../assets/img/Home/svg/clients/kaf.svg" alt="kaf">
            </a>
            <a>
              <img src="../../assets/img/Home/svg/clients/socialshopwave.svg" alt="socialshopwave">
            </a>
            <a class="small-image">
              <img src="../../assets/img/Home/svg/clients/nambafood.svg" alt="nambafood">
            </a>
            <a class="small-image">
              <img src="../../assets/img/Home/svg/clients/silkroadexplore.svg" alt="silkroadexplore">
            </a>
            <a class="lakediamond">
              <img src="../../assets/img/Home/png/clients/lakediamond@2x.png" alt="lakediamond" />
            </a>
            <a>
              <img src="../../assets/img/Home/svg/clients/idmatch.svg" alt="IdMatch">
            </a>
            <a>
              <img src="../../assets/img/Home/svg/clients/besmart.svg" alt="besmart">
            </a>
            <a>
              <img src="../../assets/img/Home/svg/clients/inn-4-pet.svg" alt="inn-4-pet">
            </a>
            <a class="GuardRails">
              <img src="../../assets/img/Home/svg/clients/GuardRails.svg" alt="GuardRails">
            </a>
            <a class="tengri">
              <img src="../../assets/img/Home/svg/clients/tengri.svg" alt="tengri">
            </a>
            <a class="photobook">
              <img src="../../assets/img/Home/svg/clients/photobook.svg" alt="photobook">
            </a>
            <a class="small-image">
              <img src="../../assets/img/Home/svg/clients/smk.svg" alt="smk">
            </a>
            <a class="small-image">
              <img src="../../assets/img/Home/svg/clients/pickd.svg" alt="pickd">
            </a>
             <a class="small-image">
              <img src="../../assets/img/Home/svg/clients/smb.svg" alt="smb">
            </a>
            <a class="small-image">
              <img src="../../assets/img/Home/svg/clients/elcart.svg" alt="elcart">
            </a>
             <a class="small-image">
              <img src="../../assets/img/Home/svg/clients/diesel.svg" alt="diesel">
            </a>
            <a class="namba-taxi">
              <img src="../../assets/img/Home/svg/clients/namba-taxi.svg" alt="namba-taxi">
            </a>
            <a class="scentomania">
              <img src="../../assets/img/Home/svg/clients/scento.svg" alt="scento">
            </a>
          </div>
        </div>
      </div>
    </div>
    <button class="clients_btn" @click="toggleLogoWrap()">
      <span v-if="!OpenWrap">
        {{ $t('All our customers') }}
        <img src="../../assets/img/Home/svg/clients/btn-icon.svg" alt="Open hide icons">
      </span>
      <span v-else>
        {{ $t('Hide') }}
        <img src="../../assets/img/Home/svg/clients/btn-icon.svg" alt="Open hide icons">
      </span>
    </button>
  </section>
</template>

<script>
export default {
  name: 'clients',
  data() {
    return {
      OpenWrap: false
    };
  },
  methods: {
    toggleLogoWrap() {
      this.OpenWrap = !this.OpenWrap;
    }
  }
};
</script>
