<template>
    <v-row justify="center" class="space px-16">
      <v-col
        cols="12"
        xs="12"
        sm="6"
        md="4"
        v-for="(product, i) in products"
        :key="i"
      >
        <v-card class="mx-auto rounded-xl" max-width="300" color="" flat outlined>
          <div align="center" justify="center">
            <v-img
              max-height="300"
              max-width="300"
              contain
              :src="product.img"
            ></v-img>
          </div>
  
          <v-card-title class="">{{ product.title }}</v-card-title>
          <v-card-title class="grey--text text-grey-darken-1 caption mt-n6">{{
            product.subtitle
          }}</v-card-title>
          <v-card-title class="mt-n4">{{ product.price }}</v-card-title>
  
          <v-card-actions class="mx-2 mt-n4">
            <v-btn outlined class="mt-n2 add">
              <v-icon color="green" @click="decrement"> mdi-minus </v-icon>
            </v-btn>
  
            <strong class="mx-2" v-text="bpm"></strong>
            <v-btn outlined class="mt-n2 add">
              <v-icon color="green" @click="increment"> mdi-plus </v-icon>
            </v-btn>
            <v-spacer></v-spacer>
            <v-btn class="mx-2 mt-n3" fab dark small color="green">
              <v-icon dark> mdi-shopping </v-icon>
            </v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
  </template>
  
  <script>
  export default {
    data: () => ({
        bpm: 1,
      products: [
        { img: "pr1.png", title: "수박", subtitle: "+9kg", price: "17,000원" },
        { img: "pr2.png", title: "무안양파", subtitle: "+2kg", price: "6,000원" },
        { img: "pr3.png", title: "햇감자", subtitle: "1kg", price: "5,000원" },
        { img: "pr4.png", title: "청송사과", subtitle: "+5kg", price: "40,000원" },
        { img: "pr5.png", title: "제주흑돼지삼겹살", subtitle: "1근", price: "26,000원" },
        { img: "pr6.png", title: "망고", subtitle: "3입 +1kg", price: "8,000원" },
      ],
    }),
     methods: {
        decrement () {
          this.bpm--
        },
        increment () {
          this.bpm++
        },
       
      },
  };
  </script>
  
  <style>
  </style>