<template>
  <div>
    <div class="intro">
      <div class="info">
        <div class="title">
          Want anything to be easy with
          <span class="needbold">LaslesVPN</span>.
        </div>
        <div class="subtitle">
          Provide a network for all your needs with ease and fun using
          <span
            class="boldvpn"
          >Lasles VPN</span> discover interesting features from us.
        </div>
        <div class="get-started full">
          <button type="submit">Get Started</button>
        </div>
      </div>
      <div class="promo-img">
        <img src="/img/promo.png" alt="promo" />
      </div>
      <div class="get-started tablet">
        <button type="submit">Get Started</button>
      </div>
    </div>
    <div class="info-stat">
      <div class="info-stat__icon">
        <img src="/img/user.png" alt />
        <div class="icon-number">
          90+
          <div class="icon-text">Users</div>
        </div>
      </div>
      <div class="info-stat__icon2">
        <img src="/img/location.png" alt />
        <div class="icon-number">
          30+
          <div class="icon-text">Locations</div>
        </div>
      </div>
      <div class="info-stat__icon">
        <img src="/img/Server.png" alt />
        <div class="icon-number">
          50+
          <div class="icon-text">Servers</div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Intro'
}
</script>

<style>
.intro {
  max-width: 1146px;
  margin: 0 auto;
  display: flex;

  margin-top: 100px;
  padding: 0px 10px 0 10px;
}

.info {
  display: flex;
  flex-direction: column;
  justify-content: space-around;
}

.title {
  font-family: Rubik;
  font-style: normal;
  font-weight: 500;
  font-size: 50px;
  line-height: 70px;
  width: 530px;
}

.needbold {
  font-weight: 700;
}

.subtitle {
  font-family: Rubik;
  font-style: normal;
  font-weight: 300;
  font-size: 16px;
  line-height: 30px;
  color: #4F5665;
}

.get-started.tablet {
  display: none;
}
.get-started button {
  padding: 17px 80px;
  border: 1px solid #F53855;
  border-radius: 10px;
  background-color: #F53855;
  color: #ffffff;
  font-weight: 700;
  box-shadow: 0px 20px 54px -14px #F53855;

}

.promo-img img {

}

.boldvpn {
  font-weight: 700;
}

.info-stat {
  max-width: 900px;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
  align-content: center;
  margin-top: 120px;
  height: 140px;
  padding: 30px 80px 30px 80px;
  box-shadow:  #f1f1f1 0px 1px 18px 4px;
}




.info-stat__icon {
  display: flex;
  align-items: center;
}

.icon-text {
  margin-top: 10px;
  font-weight: 300;
  color: #4F5665;
}

.icon-number {
  display: flex;
  flex-direction: column;
  margin-left: 38px;
}


.info-stat__icon2 {
  display: flex;
  align-items: center;
  position: relative;
}

.info-stat__icon2::before {
  content: '';
  border-left: 2px solid #EEEFF2;
  height: 125px;
  width: 2px;
  position: absolute;
  right: 260px;
}

.info-stat__icon2::after {
  content: '';
  border-left: 2px solid #EEEFF2;
  height: 125px;
  width: 2px;
  position: absolute;
  left: 260px;
}

@media only screen and (max-width: 1146px) {
  .intro {
    flex-direction: column;
  }
  .intro > *{
    margin: 0 auto;
    text-align: center;
  }
  .title {
    width: unset;
  }
  .get-started.tablet {
    display: block;
    margin-top: 50px;
  }
  .get-started.full {
    display: none;
  }
  .subtitle {
    margin-top: 20px;
  }

  .promo-img {
    margin-top: 50px;
  }
}

</style>
