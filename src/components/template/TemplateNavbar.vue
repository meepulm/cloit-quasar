<template>
  <q-header class="container row items-center absolute absolute-top">
    <div class="col">
      <q-img src="~assets/images/logo-navbar.png" width="114px" />
    </div>
    <div class="col flex justify-center">
      <q-list dense class="flex" style="gap: 60px">
        <q-btn dense unelevated label="채용">
          <q-menu>
            <q-list dense style="min-width: 100px">
              <q-item clickable v-close-popup>
                <q-item-section class="text-weight-bold">채용</q-item-section>
              </q-item>
              <q-item clickable v-close-popup>
                <q-item-section>해외 개발자 원격 채용</q-item-section>
              </q-item>
              <q-item clickable v-close-popup>
                <q-item-section>외국인 원격 채용 (비개발 직군)</q-item-section>
              </q-item>
              <q-separator />
              <q-item clickable v-close-popup>
                <q-item-section>한국어 가능 외국인 채용</q-item-section>
              </q-item>
            </q-list>
          </q-menu>
          <q-btn dense flat icon="expand_more" />
        </q-btn>

        <q-item dense clickable v-ripple class="no-padding">
          <q-item-section> 해외 개발자 활용 서비스 </q-item-section>
        </q-item>
      </q-list>
    </div>
    <div class="col flex justify-end">
      <q-btn
        class="cta"
        color="white"
        text-color="black"
        label="문의하기"
        unelevated
      />
      <q-icon name="menu" @click="open('right')" />
      <q-dialog v-model="dialog" :position="position">
        <q-card style="width: 280px; border-radius: 0px" class="q-pa-md">
          <q-list dense bordered padding class="rounded-borders">
            <q-item clickable v-ripple class="bg-blue-grey-1">
              <q-item-section class="text-weight-bolder"> 채용 </q-item-section>
            </q-item>
            <q-item clickable v-ripple>
              <q-item-section class="q-pl-lg">
                해외 개발자 원격 채용
              </q-item-section>
            </q-item>
            <q-item clickable v-ripple>
              <q-item-section class="q-pl-lg">
                외국인 원격 채용 (비개발 직군)
              </q-item-section>
            </q-item>
            <q-item clickable v-ripple>
              <q-item-section class="q-pl-lg">
                한국어 가능 외국인 채용
              </q-item-section>
            </q-item>
            <q-separator />
            <q-item clickable v-ripple>
              <q-item-section class="text-weight-bolder">
                해외 개발자 활용 서비스
              </q-item-section>
            </q-item>
            <q-item>
              <q-item-section>
                <q-btn
                  class="cta-mobile"
                  color="white"
                  text-color="black"
                  label="문의하기"
                  unelevated
                />
              </q-item-section>
            </q-item>
          </q-list>
        </q-card>
      </q-dialog>
    </div>
  </q-header>
</template>

<script>
import { defineComponent, ref } from "vue";

export default defineComponent({
  name: "TemplateNavbar",

  setup() {
    const dialog = ref(false);
    const position = ref("right");

    return {
      dialog,
      position,

      open(pos) {
        position.value = pos;
        dialog.value = true;
      },

      onItemClick() {},
    };
  },
});
</script>

<style>
.q-header {
  padding: 13px 0px;
  background: transparent;
}

.q-menu .q-list .q-item:last-child {
  border-top: 1px solid #f2f4f7;
}

.q-btn .q-icon,
.q-btn .q-spinner {
  font-size: 18px;
}

.q-list--dense > .q-item,
.q-item--dense {
  padding: 10px 16px;
}

.q-header .cta {
  border-radius: 8px;
  padding: 6px 24px;
  font-weight: 900;
  color: #4a77ff !important;
  display: block;
}

.q-icon {
  display: none;
}

@media (max-width: 768px) {
  .container {
    padding: 20px 16px;
  }
  .q-header .col:nth-child(2) {
    display: none;
  }

  .q-header .cta {
    display: none;
  }

  .q-icon {
    display: block;
    font-size: 26px;
  }

  .cta-mobile {
    padding: 6px 24px;
    width: 100%;
    color: #fff !important;
    font-weight: 900;
    background-color: #26c2b9 !important;
  }

  .q-dialog__inner--minimized {
    padding: 0px !important;
  }

  .q-dialog .q-card {
    height: 100vh !important;
    max-height: unset !important;
  }
}
</style>
