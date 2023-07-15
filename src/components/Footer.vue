<template>
  <v-footer dark padless>
    <v-card flat tile class="black white--text py-12 px-5" width="100%">
      <v-row>
        <v-col cols="12" xs="12" sm="6" md="4" class="pa-16">
          <v-toolbar color="transparent" flat>
            <v-badge color="#D5F0DB" dot>
              <v-img src="1.png" contain width="30"></v-img>
            </v-badge>

            <v-toolbar-title class="ml-4">
              <span class="green--text">e</span><strong>동네식료품</strong>
            </v-toolbar-title>
          </v-toolbar>
          <v-card-text class="pt-0">
            <v-btn
              v-for="icon in icons"
              :key="icon"
              class="mx-1 white--text"
              icon
              fab
              outlined
              small
            >
              <v-icon size="20px">
                {{ icon }}
              </v-icon>
            </v-btn>
          </v-card-text>
        </v-col>
        <v-col cols="12" xs="12" sm="6" md="2">
          <v-card-text class="white--text pt-0">
            <h3>About</h3>
          </v-card-text>
          <v-card-text class="grey--text">점포 소개</v-card-text>
          <v-card-text class="grey--text mt-n4">주문 방법</v-card-text>
          <v-card-text class="grey--text mt-n4">특가 세일</v-card-text>
          <v-card-text class="grey--text mt-n4">친구 소개</v-card-text>
        </v-col>
        <v-col cols="12" xs="12" sm="6" md="2">
          <v-card-text class="white--text pt-0">
            <h3>Dellvery</h3>
          </v-card-text>
          <v-card-text class="grey--text">배달 관련</v-card-text>
          <v-card-text class="grey--text mt-n4">지불 방법</v-card-text>
          <v-card-text class="grey--text mt-n4">진행 상태</v-card-text>
          <v-card-text class="grey--text mt-n4">반품 관련</small></v-card-text>
        </v-col>
        <v-col cols="12" xs="12" sm="6" md="4">
          <v-card-text class="white--text pt-0">
            <h3>Contact</h3>
          </v-card-text>
          <v-card-text class="grey--text">동네식료품</v-card-text>
          <v-card-text class="grey--text mt-n4">
            서울시 성동구 성수 1로 77 1F
          </v-card-text>
          <v-card-text class="grey--text mt-n4">bestgrocery.co.kr</v-card-text>
          <v-card-text class="grey--text mt-n4">010-333-7777</v-card-text>
        </v-col>
      </v-row>
    </v-card>
  </v-footer>
</template>

<script>
export default {
  data: () => ({
    icons: [
      "fab fa-apple",
      "fab fa-google-plus-g",
      "fab fa-twitter",
      "fab fa-facebook-f",
    ],
  }),
};
</script>

<style>
</style>