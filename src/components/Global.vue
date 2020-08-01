<template>
  <div>
     <div class="global">
      <div class="global-title">Huge Global Network of Fast VPN</div>
      <div class="global-subtitle">See <span class="boldvpn">Lasles VPN</span> everywhere to make it easier for you when you move locations.</div>
      <div class="global-map"><img src="/img/Huge Global.png" alt=""></div>
    </div>
    <div class="for-apps">
      <div class="for-apps-img"><img src="/img/Mask Group (1).png" alt=""></div>
      <div class="for-apps-img"><img src="/img/Mask Group (2).png" alt=""></div>
      <div class="for-apps-img"><img src="/img/Mask Group (3).png" alt=""></div>
      <div class="for-apps-img"><img src="/img/Mask Group.png" alt=""></div>
    </div>
  </div>
</template>

<script>
export default {
  name:'Global'
}
</script>

<style>
  .global {
  max-width: 1146px;
  margin: 0 auto;
  margin-top: 150px;
}

.global-title {
  text-align: center;
  font-family: Rubik;
  font-style: normal;
  font-weight: 500;
  font-size: 35px;
  line-height: 50px;
  text-align: center;
  color: #0B132A;
  width: 380px;
  margin: 0 auto;
}

.global-subtitle {
  font-family: Rubik;
  font-style: normal;
  font-weight: 300;
  font-size: 16px;
  line-height: 30px;
  text-align: center;
  color: #4F5665;
  margin: 0 auto;
  padding-top: 20px;
  width: 380px;
}

.global-map {
  text-align: center;
  margin-top: 150px;
}

.for-apps {
  display: flex;
  justify-content: space-around;
  max-width: 1146px;
  margin: 0 auto;
  align-items: center;
  margin-top: 110px;
}

.for-apps-img {

}
</style>
