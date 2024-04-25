<template>
  <div class="hero">
    <div class="container">
      <div class="row items-center" style="gap: 70px">
        <div class="col column" style="gap: 60px">
          <div class="column" style="gap: 24px">
            <div class="intro column" style="gap: 16px">
              <transition
                appear
                enter-active-class="animated fadeIn duration-500 delay-3s"
              >
                <div class="label">풀타임, 파트타임</div>
              </transition>
              <transition
                appear
                enter-active-class="animated fadeInUp duration-500"
              >
                <h1>
                  최고의 실력을 가진<br />
                  외국인 인재를 찾고 계신가요?
                </h1>
              </transition>
              <transition
                appear
                enter-active-class="animated fadeInUp duration-500"
              >
                <p class="q-animate fadeInUp duration-500">
                  법률 및 인사관리 부담없이<br />
                  1주일 이내에 원격으로 채용해보세요.
                </p>
              </transition>
            </div>
            <p class="question">개발자가 필요하신가요?</p>
          </div>
          <div class="row count" style="gap: 48px">
            <div class="col column usp" style="gap: 8px">
              <h6>평균 월 120만원</h6>
              <p>임금을 해당 국가를 기준 으로 계산합니다.</p>
            </div>
            <div class="col column usp" style="gap: 8px">
              <h6>평균 월 120만원</h6>
              <p>임금을 해당 국가를 기준 으로 계산합니다.</p>
            </div>
            <div class="col column usp" style="gap: 8px">
              <h6>평균 월 120만원</h6>
              <p>임금을 해당 국가를 기준 으로 계산합니다.</p>
            </div>
          </div>
        </div>
        <transition appear enter-active-class="animated fadeIn duration-500">
          <div class="col">
            <div class="label profit">
              <q-img src="~assets/images/icons/icon-dollar.svg" width="26px" />
              <p>월 100만원</p>
            </div>
            <swiper
              :effect="'coverflow'"
              :grabCursor="true"
              :centeredSlides="true"
              :loop="true"
              :navigation="true"
              :slidesPerView="2"
              :coverflowEffect="{
                rotate: 50,
                stretch: 0,
                depth: 100,
                modifier: 1,
                slideShadows: false,
              }"
              :modules="modules"
              class="card-carousel"
            >
              <swiper-slide v-for="index in 7" :key="index">
                <q-card flat>
                  <q-card-section class="column items-center" style="gap: 36px">
                    <div class="column items-center" style="gap: 16px">
                      <div class="relative-position" style="width: fit-content">
                        <q-avatar size="120px">
                          <img src="~assets/images/avatar.png" />
                        </q-avatar>
                        <q-img
                          class="absolute absolute-bottom-right"
                          src="~assets/images/flag.png"
                          width="25px"
                        />
                      </div>
                      <div class="column items-center text-center">
                        <h6>Abhishek Gupta</h6>
                        <p>마케팅 · 2y+</p>
                      </div>
                    </div>
                    <div class="flex justify-center" style="gap: 4px">
                      <q-badge outline label="마케팅 콘텐츠 제작" />
                      <q-badge outline label="인스타그램 관리" />
                      <q-badge outline label="트위터 관리" />
                      <q-badge outline label="블로그 글 작성" />
                    </div>
                  </q-card-section>
                </q-card>
              </swiper-slide>
            </swiper>
            <div class="feature-mobile">
              <div class="column" style="gap: 12px">
                <div class="flex items-center" style="gap: 16px">
                  <div class="flex items-center" style="gap: 12px">
                    <q-img
                      src="~assets/images/icons/icon-checkbox.svg"
                      width="20px"
                    />
                    <p>한국어 능력</p>
                  </div>
                  <div class="flex items-center" style="gap: 12px">
                    <q-img
                      src="~assets/images/icons/icon-checkbox.svg"
                      width="20px"
                    />
                    <p>업무 수행 능력</p>
                  </div>
                </div>
                <div class="flex items-center" style="gap: 16px">
                  <div class="flex items-center" style="gap: 12px">
                    <q-img
                      src="~assets/images/icons/icon-checkbox.svg"
                      width="20px"
                    />
                    <p>겸업 여부</p>
                  </div>
                  <div class="flex items-center" style="gap: 12px">
                    <q-img
                      src="~assets/images/icons/icon-checkbox.svg"
                      width="20px"
                    />
                    <p>평판 조회</p>
                  </div>
                </div>
              </div>
              <p>개발자가 필요하신가요?</p>
            </div>
          </div>
        </transition>
      </div>
    </div>
    <transition appear enter-active-class="animated fadeIn duration-500">
      <swiper
        :spaceBetween="10"
        :slidesPerView="'auto'"
        :autoplay="{
          delay: 5000,
          disableOnInteraction: false,
        }"
        :modules="modules"
        class="feature-carousel"
      >
        <swiper-slide>
          <div class="item">
            <div class="icon-wrapper">
              <q-img
                src="~assets/images/icons/icon-marketing.svg"
                width="32px"
              />
            </div>
            <p>해외 마케팅</p>
          </div>
        </swiper-slide>
        <swiper-slide>
          <div class="item">
            <div class="icon-wrapper">
              <q-img src="~assets/images/icons/icon-image.svg" width="32px" />
            </div>
            <p>퍼블리셔</p>
          </div>
        </swiper-slide>
        <swiper-slide>
          <div class="item">
            <div class="icon-wrapper">
              <q-img src="~assets/images/icons/icon-box.svg" width="32px" />
            </div>
            <p>캐드원(제도사)</p>
          </div>
        </swiper-slide>
        <swiper-slide>
          <div class="item">
            <div class="icon-wrapper">
              <q-img src="~assets/images/icons/icon-target.svg" width="32px" />
            </div>
            <p>해외 세일즈</p>
          </div>
        </swiper-slide>
        <swiper-slide>
          <div class="item">
            <div class="icon-wrapper">
              <q-img src="~assets/images/icons/icon-call.svg" width="32px" />
            </div>
            <p>해외 CS</p>
          </div>
        </swiper-slide>
        <swiper-slide>
          <div class="item">
            <div class="icon-wrapper">
              <q-img
                src="~assets/images/icons/icon-marketing.svg"
                width="32px"
              />
            </div>
            <p>해외 마케팅</p>
          </div>
        </swiper-slide>
      </swiper>
    </transition>
  </div>
</template>

<script>
import { defineComponent } from "vue";
import { Swiper, SwiperSlide } from "swiper/vue";
import "swiper/css";
import "swiper/css/effect-coverflow";
import "swiper/css/navigation";
import { EffectCoverflow, Navigation } from "swiper/modules";

export default defineComponent({
  name: "IndexPage",
  components: {
    Swiper,
    SwiperSlide,
  },
  setup() {
    return {
      modules: [EffectCoverflow, Navigation],
    };
  },
});
</script>

<style>
.hero {
  background: linear-gradient(151.17deg, #26c2b9 8.69%, #288be7 126.06%);
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  background-blend-mode: color-burn;
  padding-top: 120px;
  height: 100vh;
}

.hero .label {
  font-size: 18px;
  font-weight: 900;
  line-height: 1.5;
  color: #40e2e8;
  background-color: #fff;
  padding: 6px 12px;
  width: fit-content;
  border-radius: 8px;
  position: relative;
  margin-bottom: 16px;
}

.hero .label::after {
  content: "";
  position: absolute;
  bottom: -16px;
  left: 16px;
  border-left: 8px solid transparent;
  border-right: 8px solid transparent;
  border-top: 8px solid #fff;
  border-bottom: 8px solid transparent;
}

.hero .label.profit {
  display: flex;
  align-items: center;
  gap: 10px;
  padding: 8px 16px;
  color: #00c696;
  margin: 0px auto 32px auto;
}

.hero .label.profit::after {
  left: 50%;
  transform: translateX(-50%);
}

.hero .intro h1 {
  font-size: 48px;
  font-weight: 900;
  line-height: 1.3;
  color: #fff;
}

.hero .intro p {
  font-size: 24px;
  line-height: 34px;
  font-weight: 900;
  color: #fff;
}

.hero .question {
  font-size: 18px;
  line-height: 1.5;
  font-weight: 900;
  color: #fff;
  text-decoration: underline;
}

.hero .usp {
  padding-top: 8px;
  border-top: 1px solid #fff;
  color: #fff;
}

.hero .usp h6 {
  font-size: 18px;
  line-height: 1.5;
  font-weight: 900;
}

.hero .usp p {
  font-size: 16px;
  line-height: 1.5;
  font-weight: 900;
}

.hero .swiper .q-card {
  border-radius: 12px;
  box-shadow: 0px 15px 24px 0px rgba(0, 0, 0, 0.12) !important;
}

.hero .swiper .q-card .q-card__section {
  padding: 36px 26px;
}

.hero .swiper .q-card h6 {
  font-size: 24px;
  line-height: 1.5;
  font-weight: 900;
  color: #24252f;
}

.hero .swiper .q-card p {
  font-size: 16px;
  line-height: 1.5;
  font-weight: 900;
  color: #4a77ff;
}

.hero .swiper .q-card .q-badge {
  border: 1px solid #c1c5cf;
  border-radius: 6px;
  color: #5e626f;
  padding: 4px 12px;
  font-size: 16px;
  line-height: 1.5;
  font-weight: 900;
}

.hero .feature-mobile {
  display: none;
}

@media (max-width: 768px) {
  .hero {
    height: auto;
    padding-bottom: 60px;
  }

  .hero .intro h1 {
    font-size: 36px;
  }

  .hero .row {
    flex-direction: column;
  }

  .hero .count {
    display: none;
  }

  .hero .question {
    display: none;
  }

  .hero .swiper .q-card h6 {
    font-size: 18px;
  }

  .hero .swiper .q-card p {
    font-size: 14px;
  }

  .hero .swiper .q-card .q-badge {
    font-size: 14px;
  }

  .hero .feature-mobile {
    display: flex;
    flex-direction: column;
    gap: 16px;
    margin-top: 26px;
  }

  .hero .feature-mobile .column p,
  .hero .feature-mobile > p {
    font-size: 16px;
    line-height: 1.5;
    font-weight: 900;
    color: #fff;
  }

  .hero .feature-mobile > p {
    color: #fbff23;
    text-decoration: underline;
  }
}
</style>
