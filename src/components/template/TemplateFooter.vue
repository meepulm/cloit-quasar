<template>
  <q-footer>
    <div class="container column" style="gap: 46px">
      <div class="row">
        <div class="col-4 column" style="gap: 18px">
          <div class="intro-top column" style="gap: 16px">
            <q-img src="~assets/images/logo-footer.png" width="187px" />
            <p>우리는 국가의 장벽을 넘어 최고의 인재를 매칭해드립니다.</p>
          </div>
          <div class="intro-bot column" style="gap: 8px">
            <p>010-0000-0000</p>
            <p>aaaaa@naver.com</p>
          </div>
        </div>
        <div class="col-8 q-pl-md">
          <div class="row" style="gap: 15px">
            <div class="col">
              <q-card flat>
                <q-card-section class="column" style="gap: 16px">
                  <div class="column" style="gap: 12px">
                    <div class="icon-wrapper">
                      <q-img
                        src="~assets/images/icons/icon-code.svg"
                        width="24px"
                      />
                    </div>
                    <p>해외 개발자 원격 채용</p>
                  </div>
                  <div class="flex items-center" style="gap: 4px">
                    <p style="color: #5e626f">바로가기</p>
                    <q-img
                      src="~assets/images/icons/icon-detail.svg"
                      width="20px"
                    />
                  </div>
                </q-card-section>
              </q-card>
            </div>
            <div class="col">
              <q-card flat>
                <q-card-section class="column" style="gap: 16px">
                  <div class="column" style="gap: 12px">
                    <div class="icon-wrapper">
                      <q-img
                        src="~assets/images/icons/icon-avatar.svg"
                        width="24px"
                      />
                    </div>
                    <p>외국인 원격 채용 (비개발)</p>
                  </div>
                  <div class="flex items-center" style="gap: 4px">
                    <p style="color: #5e626f">바로가기</p>
                    <q-img
                      src="~assets/images/icons/icon-detail.svg"
                      width="20px"
                    />
                  </div>
                </q-card-section>
              </q-card>
            </div>
            <div class="col">
              <q-card flat>
                <q-card-section class="column" style="gap: 16px">
                  <div class="column" style="gap: 12px">
                    <div class="icon-wrapper">
                      <q-img
                        src="~assets/images/icons/icon-kor.svg"
                        width="24px"
                      />
                    </div>
                    <p>한국어 가능 외국인 채용</p>
                  </div>
                  <div class="flex items-center" style="gap: 4px">
                    <p style="color: #5e626f">바로가기</p>
                    <q-img
                      src="~assets/images/icons/icon-detail.svg"
                      width="20px"
                    />
                  </div>
                </q-card-section>
              </q-card>
            </div>
            <div class="col">
              <q-card flat>
                <q-card-section class="column" style="gap: 16px">
                  <div class="column" style="gap: 12px">
                    <div class="icon-wrapper">
                      <q-img
                        src="~assets/images/icons/icon-gear.svg"
                        width="24px"
                      />
                    </div>
                    <p>해외 개발자 활용 서비스</p>
                  </div>
                  <div class="flex items-center" style="gap: 4px">
                    <p style="color: #5e626f">바로가기</p>
                    <q-img
                      src="~assets/images/icons/icon-detail.svg"
                      width="20px"
                    />
                  </div>
                </q-card-section>
              </q-card>
            </div>
          </div>
        </div>
      </div>
      <div class="row menu">
        <div class="col-2 column" style="gap: 10px">
          <p class="menu-title">상호명</p>
          <div class="column" style="gap: 5px">
            <p class="menu-desc">하이퍼하이어</p>
            <p class="menu-desc">Hyperhire India Private Limited</p>
          </div>
        </div>
        <div class="col-2 column q-pl-lg" style="gap: 10px">
          <p class="menu-title">대표 CEO</p>
          <div class="column" style="gap: 5px">
            <p class="menu-desc">김주현</p>
            <p class="menu-desc">Juhyun Kim</p>
          </div>
        </div>
        <div class="col-12 col-md-2 column q-pl-lg" style="gap: 10px">
          <p class="menu-title">사업자등록번호 CIN</p>
          <div class="column" style="gap: 5px">
            <p class="menu-desc">427-86-01187</p>
            <p class="menu-desc">U74110DL2016PTC290812</p>
          </div>
        </div>
        <div class="col-12 col-md-6 column q-pl-lg" style="gap: 10px">
          <p class="menu-title">주소 ADDRESS</p>
          <div class="column" style="gap: 5px">
            <p class="menu-desc">서울특별시 강남대로 479, 지하 1층 238호</p>
            <p class="menu-desc">
              D-138, Street number 11, Jagjeet Nagar, North East Delhi, New
              Delhi, 110053 India
            </p>
          </div>
        </div>
      </div>
      <p>ⓒ {{ new Date().getFullYear() }} Hyperhire</p>
    </div>
  </q-footer>
</template>

<script>
import { defineComponent } from "vue";

export default defineComponent({
  name: "TemplateFooter",
});
</script>

<style>
.q-footer {
  position: relative;
  padding: 80px 0px;
  background-color: #fbfbfb;
  color: #343741;
}

.q-footer .intro-top p {
  font-size: 14px;
  line-height: 1.5;
  font-weight: 900;
}

.q-footer .intro-bot p {
  font-size: 13px;
  line-height: 1.5;
  font-weight: 900;
  color: #5e626f;
}

.q-footer .q-card {
  border-radius: 12px;
}

.q-footer .q-card .q-card__section {
  padding: 16px;
}

.q-footer .q-card .icon-wrapper {
  padding: 8px;
  border-radius: 8px;
  background-color: #eff1f6;
  width: fit-content;
}

.q-footer .q-card p {
  font-size: 14px;
  line-height: 1.5;
  font-weight: 900;
}

.q-footer .menu-title {
  font-size: 12px;
  line-height: 1.5;
  font-weight: 900;
}

.q-footer .menu-desc {
  font-size: 13px;
  line-height: 1.5;
  font-weight: 900;
  color: #5e626f;
}

.q-footer .container > p {
  font-size: 13px;
  line-height: 1.5;
  font-weight: 900;
  color: #5e626f;
}

@media (max-width: 768px) {
  .q-footer .row .col-4 {
    width: 100%;
  }

  .q-footer .row .col-8 {
    margin-top: 18px;
    padding-left: 0px;
    width: 100%;
  }

  .q-footer .row .col-8 .row {
    flex-direction: row;
  }

  .q-footer .row .col-8 .row .col {
    flex: 0 0 auto;
    width: calc(50% - 8px);
  }

  .q-footer .menu .column {
    padding-left: 0px;
  }

  .q-footer .menu > .col-2.column:first-child,
  .q-footer .menu > .col-2.column:nth-child(2) {
    width: calc(50% - 10px);
  }

  .q-footer .menu > .column:nth-child(3),
  .q-footer .menu > .column:last-child {
    width: 100%;
    margin-top: 36px;
  }
}
</style>
