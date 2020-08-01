<template>
   <div class="terms">
      <div class="terms-human"><img src="/img/human.png" alt=""></div>
      <div class="terms-info">
        <div class="terms-title">We Provide Many Features You Can Use</div>
        <div class="terms-subtitle">You can explore the features that we provide with fun and have their own functions each feature.</div>
      <div class="terms-content-box">
        <div class="terms-content"><img src="/img/check.png" alt="">Powerfull online protection.</div>
        <div class="terms-content"><img src="/img/check.png" alt="">Internet without borders.</div>
        <div class="terms-content"><img src="/img/check.png" alt="">Supercharged VPN.</div>
        <div class="terms-content"><img src="/img/check.png" alt="">No specific time limits.</div>
      </div>
      </div>
    </div>
</template>

<script>
export default {
  name: 'Terms'
}
</script>

<style>
.terms {
  display: flex;
  max-width: 1146px;
  margin: 0 auto;
  margin-top: 96px;
  align-items: center;
  justify-content: space-between;
  margin-bottom: 130px;
}

.terms-info {
  display: flex;
  flex-direction: column;
}

.terms-title {
  font-family: Rubik;
  font-style: normal;
  font-weight: 500;
  font-size: 35px;
  line-height: 50px;
  width: 380px;
  color: #0B132A;
  margin-top: 48px;
}

.terms-subtitle {
  font-family: Rubik;
  font-style: normal;
  font-size: 16px;
  line-height: 30px;
  width: 410px ;
  color: #4F5665;
  font-weight: 300;
  margin-top: 20px;
}

.terms-content {
  font-family: Rubik;
  font-style: normal;
  font-weight: 300;
  font-size: 14px;
  line-height: 30px;
  color: #4F5665;
  display: flex;
  align-items: center;
  margin-top: 15px ;
}

.terms-content-box{
  display: flex;
  flex-direction: column;
  margin-top: 20px;

}

.terms-content img {
  margin-right: 10px;
}
</style>

