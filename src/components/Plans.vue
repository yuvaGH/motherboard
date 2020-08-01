<template>
    <div class="plans-backgroun">
    <div class="plans">
      <div class="plans-intro-block">
        <div class="plans-title">Choose Your Plan</div>
        <div class="plans-subtitle">Let's choose the package that is best for you and explore it happily and cheerfully.</div>
      </div>
      <div class="plans-plans">
        <div class="info-plan">
          <div class="box">
            <img src="/img/Free.png" alt="">
            <div class="title-plan">Free Plan</div>
          </div>
            <div class="plan-list">
              <div class="plan-content"><img src="/img/plancheck.png" alt="">Unlimited Bandwitch</div>
              <div class="plan-content"><img src="/img/plancheck.png" alt="">Encrypted Connection</div>
              <div class="plan-content"><img src="/img/plancheck.png" alt="">No Traffic Logs</div>
              <div class="plan-content"><img src="/img/plancheck.png" alt="">Works on All Devices</div>
            </div>
            <div class="plans-actions">
              <div class="plans-actions__price">Free</div>
              <div class="plans-actions__select"><button type="submit">Select</button></div>
            </div>
        </div>
        <div class="info-plan">
          <div class="box">
            <img src="/img/Standard.png" alt="">
            <div class="title-plan">Standart Plan</div>
          </div>
          <div class="plan-list">
            <div class="plan-content"><img src="/img/plancheck.png" alt="">Unlimited Bandwitch</div>
            <div class="plan-content"><img src="/img/plancheck.png" alt="">Encrypted Connection</div>
            <div class="plan-content"><img src="/img/plancheck.png" alt="">No Traffic Logs</div>
            <div class="plan-content"><img src="/img/plancheck.png" alt="">Works on All Devices</div>
            <div class="plan-content"><img src="/img/plancheck.png" alt="">Connect Anyware</div>
          </div>
          <div class="plans-actions">
            <div class="plans-actions__price">$9 / mo</div>
            <div class="plans-actions__select"><button type="submit">Select</button></div>
          </div>
        </div>
        <div class="info-plan premium">
          <div class="box">
            <img src="/img/Premium.png" alt="">
            <div class="title-plan">Premium Plan</div>
          </div>
          <div class="plan-list">
            <div class="plan-content"><img src="/img/plancheck.png" alt="">Unlimited Bandwitch</div>
            <div class="plan-content"><img src="/img/plancheck.png" alt="">Encrypted Connection</div>
            <div class="plan-content"><img src="/img/plancheck.png" alt="">No Traffic Logs</div>
            <div class="plan-content"><img src="/img/plancheck.png" alt="">Works on All Devices</div>
            <div class="plan-content"><img src="/img/plancheck.png" alt="">Connect Anyware</div>
            <div class="plan-content"><img src="/img/plancheck.png" alt="">Get New Features</div>
          </div>
          <div class="plans-actions">
            <div class="plans-actions__price">$12 / mo</div>
            <div class="plans-actions__select premium"><button type="submit">Select</button></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name:'Plans'
}
</script>

<style>
  .plans {

  max-width: 1146px;
  margin: 0 auto;
}
.plans-intro-block {
  max-width: 1146px;
}

.plans-title {
  font-family: Rubik;
  font-style: normal;
  font-weight: 500;
  font-size: 35px;
  line-height: 50px;
  text-align: center;
  color: #0B132A;
  padding-bottom: 20px;
}

.plans-subtitle {
  font-family: Rubik;
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 30px;
  color: #4F5665;
  margin: 0 auto;
  width: 555px;
  text-align: center;
}

.plans-plans {
  display: flex;
  justify-content: space-between;
  margin-top: 60px;
}


.info-plan {
  width: 330px;
  height: 760px;
  display: flex;
  flex-direction: column;
  border: 1px solid  rgb(185, 181, 181);
  border-radius: 10px;
  align-items: center;
}

.info-plan.premium {
  border: 1px solid #F53855;
}
.info-plan .box {
  margin: 97px 0 30px 0;
}
.info-plan .box img {
  margin-bottom: 30px;
}

.title-plan {
  font-family: Rubik;
  font-style: normal;
  font-weight: 500;
  font-size: 18px;
  line-height: 30px;
  text-align: center;
  color: #0B132A;
}

.plan-content {
  font-family: Rubik;
  font-style: normal;
  font-weight: normal;
  font-size: 14px;
  line-height: 30px;
  color: #4F5665;
  display: flex;
  align-content: center;
}

.plan-content img {
  margin-right: 30px;
}

.plans-actions {
  margin: auto 0 50px 0;
}
.plans-actions > div:first-child {
  margin-bottom: 20px;
}
.plans-actions__price {
  font-family: Rubik;
  font-style: normal;
  font-weight: 500;
  font-size: 25px;
  line-height: 30px;
  text-align: center;
  color: #0B132A;
}

.plan-list {

}

.plans-actions__select button {
  padding: 13px 45px;
  border: 1px solid #F53855;
  border-radius: 50px;
  background-color: unset;
  color: #F53855;
  font-weight: 700;
}

.plans-actions__select .premium button {
  background-color: #F53855;
  color: #ffffff;
  box-shadow: 0px 20px 54px -14px #F53855;
}
</style>
