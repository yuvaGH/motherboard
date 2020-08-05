<template>
  <div class="feedback">
      <div class="feedback-title">Trusted by Thousands of Happy Customer</div>
      <div class="feedback-subtitle">These are the stories of our customers who have joined us with great pleasure when using this crazy feature.</div>
      <div class="slider">
        <div class="slider-container">
          <div v-for="(item, index) of sliderContainer" :key="index">
            <div class="container-content">
              <div class="user-info">
                <img :src="item.img" alt="">
                <div class="user-name"> {{item.name}}<br> <span class="city">{{item.city}}</span>  </div>
                <div class="user-score">{{item.score}} <img src="/img/Vector.png" alt=""></div>
              </div>
              <div class="user-comment" v-text="item.comment"></div>
            </div>
          </div>
        </div>
        <div class="slider-footer">
          <div class="slider-footer__dots">
            <div
              v-for="index in 4"
              :key="index"
              :class="index === currentPos ? 'active' : ''"
            />
          </div>
          <div class="slider-footer__arrows">
            <div class="left" @click="click('left')">
              <svg id="svg-left" width="30" height="30" viewBox="0 0 30 30" fill="white" xmlns="http://www.w3.org/2000/svg">
                <path d="M6.25 14.0028H21.075L16.5375 8.55279C16.3253 8.29751 16.2232 7.96841 16.2537 7.63788C16.2842 7.30735 16.4447 7.00246 16.7 6.79029C16.9553 6.57811 17.2844 6.47604 17.6149 6.50651C17.9454 6.53698 18.2503 6.69752 18.4625 6.95279L24.7125 14.4528C24.7545 14.5124 24.7922 14.5751 24.825 14.6403C24.825 14.7028 24.825 14.7403 24.9125 14.8028C24.9692 14.9461 24.9988 15.0987 25 15.2528C24.9988 15.4069 24.9692 15.5595 24.9125 15.7028C24.9125 15.7653 24.9125 15.8028 24.825 15.8653C24.7922 15.9305 24.7545 15.9931 24.7125 16.0528L18.4625 23.5528C18.345 23.6939 18.1978 23.8074 18.0314 23.8851C17.8651 23.9629 17.6836 24.0031 17.5 24.0028C17.2079 24.0034 16.9249 23.9016 16.7 23.7153C16.5734 23.6103 16.4688 23.4815 16.3921 23.336C16.3154 23.1906 16.2682 23.0315 16.2531 22.8678C16.238 22.704 16.2553 22.5389 16.3041 22.3819C16.3529 22.2249 16.4322 22.0791 16.5375 21.9528L21.075 16.5028H6.25C5.91848 16.5028 5.60054 16.3711 5.36612 16.1367C5.13169 15.9022 5 15.5843 5 15.2528C5 14.9213 5.13169 14.6033 5.36612 14.3689C5.60054 14.1345 5.91848 14.0028 6.25 14.0028Z" fill="#F53838"/>
                </svg>
            </div>
            <div class="right" @click="click('right')">
              <svg id="svg-right" width="30" height="30" viewBox="0 0 30 30" fill="white" xmlns="http://www.w3.org/2000/svg">
                <path d="M6.25 14.0028H21.075L16.5375 8.55279C16.3253 8.29751 16.2232 7.96841 16.2537 7.63788C16.2842 7.30735 16.4447 7.00246 16.7 6.79029C16.9553 6.57811 17.2844 6.47604 17.6149 6.50651C17.9454 6.53698 18.2503 6.69752 18.4625 6.95279L24.7125 14.4528C24.7545 14.5124 24.7922 14.5751 24.825 14.6403C24.825 14.7028 24.825 14.7403 24.9125 14.8028C24.9692 14.9461 24.9988 15.0987 25 15.2528C24.9988 15.4069 24.9692 15.5595 24.9125 15.7028C24.9125 15.7653 24.9125 15.8028 24.825 15.8653C24.7922 15.9305 24.7545 15.9931 24.7125 16.0528L18.4625 23.5528C18.345 23.6939 18.1978 23.8074 18.0314 23.8851C17.8651 23.9629 17.6836 24.0031 17.5 24.0028C17.2079 24.0034 16.9249 23.9016 16.7 23.7153C16.5734 23.6103 16.4688 23.4815 16.3921 23.336C16.3154 23.1906 16.2682 23.0315 16.2531 22.8678C16.238 22.704 16.2553 22.5389 16.3041 22.3819C16.3529 22.2249 16.4322 22.0791 16.5375 21.9528L21.075 16.5028H6.25C5.91848 16.5028 5.60054 16.3711 5.36612 16.1367C5.13169 15.9022 5 15.5843 5 15.2528C5 14.9213 5.13169 14.6033 5.36612 14.3689C5.60054 14.1345 5.91848 14.0028 6.25 14.0028Z" fill="white"/>
                </svg>
            </div>
          </div>
        </div>
      </div>
    </div>
</template>

<script>
export default {
  name: 'Feedback',
  data: () => ({
    currentPos: 1,
    sliderContainer: [
      { img: '/img/Ellipse 175.png' ,
        name: 'Viezh Rober',
        city: 'Warsaw Poland',
        score: 4.5,
        comment: '“Wow... I am very happy to use this VPN, it turned out to be more than my expectations and so far there have been no problems. LaslesVPN always the best"',
      },
      {
        img: '/img/Ellipse 175 (1).png' ,
        name: 'Yessica Christy',
        city: 'Shanxi, China',
        score: 4.5,
        comment: '“I like it because I like to travel far and still can connect with high speed.”',
      },
       {
        img: '/img/Ellipse 175 (2).png' ,
        name: 'Kim Young Jou',
        city: 'Seoul, South Korea',
        score: 4.5,
        comment: '“This is very unusual for my business that currently requires a virtual private network that has high security.”',
      },
      {
        img: '/img/Ellipse 175 (1).png' ,
        name: 'Yessica Christy',
        city: 'Shanxi, China',
        score: 4.5,
        comment: '“I like it because I like to travel far and still can connect with high speed.”',
      },
    ],
  }),
  methods: {
    click(side) {
      if (side === 'right' && this.currentPos < 4) {
        this.currentPos++;
      }
      if (side === 'left' && this.currentPos > 1) {
        this.currentPos--;
      }
    },
  },
}
</script>

<style>
  .feedback-title {
  font-family: Rubik;
  font-style: normal;
  font-weight: 500;
  font-size: 35px;
  line-height: 50px;
  text-align: center;
  max-width: 448px;
  margin: 0 auto;
  margin-top: 124px;
}

.feedback-subtitle {
  font-family: Rubik;
  font-style: normal;
  font-weight: normal;
  font-size: 16px;
  line-height: 30px;
  text-align: center;
  color: #4F5665;
  margin: 0 auto;
  margin-top: 25px;
  max-width: 555px;
}

.slider {
  display: flex;
  justify-content: space-around;
  max-width: 1390px;
  margin: 0 auto;
  align-items: center;
  margin-top: 60px;
  overflow: hidden;
  flex-direction: column;
}
.slider > div {

}

.slider-container {
  display: flex;
  margin-left: 500px;
}
.slider-container > div {
  height: 230px;
  width: 400px;
  border: 2px solid #DDDDDD;
  border-radius: 10px;
  margin-right: 50px;
  text-align: left;
}


.container-content {
  display: flex;
  flex-direction: column;
  padding: 30px 30px;

}

.user-info {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.user-name {
  right: 45px;
  position: relative;
  font-family: Rubik;
  font-style: normal;
  font-weight: 500;
  font-size: 18px;
}

.city {
  font-family: Rubik;
  color: #4F5665;
  font-size: 14px;
  font-weight: 300;
}

.user-comment {
  font-family: Rubik;
  font-weight: 300;
  font-size: 16px;
  line-height: 30px;
  align-items: center;
  color: #0B132A;
  margin-top: 10px;

}

.user-score {
  font-family: Rubik;
  font-style: normal;
  font-weight: 300;
  font-size: 16px;
  line-height: 30px;
  color: #0B132A;
}

.user-score img {
  padding-left: 10px;
}

.slider-footer {
  max-width: 1140px;
  display: flex;
  width: 100%;
}

.slider-footer__arrows {
  max-width: 1140px;
  display: flex;
  width: 100%;
  justify-content: flex-end;
  position: relative;
  margin-top: 60px ;
}

.left, .right {
  display: flex;
  align-self: self-end;
  border: 2px solid #F53838;
  box-sizing: border-box;
  padding: 20px 20px;
  border-radius: 50px;
}
.left {
  transform: rotate(180deg);
  color: #F53838;
  background: none;
  margin-right: 30px;
}

.right {
  background: #F53838;
}

.slider-footer__dots {
  display: flex;
}
.slider-footer__dots div{
  background-image: url(../../public/img/dot.png);
  background-repeat: no-repeat;
  width: 15px;
  height: 16px;
}
.slider-footer__dots div.active {
  background-image: url(../../public/img/longDot.png);
  width: 46px;
}


</style>
