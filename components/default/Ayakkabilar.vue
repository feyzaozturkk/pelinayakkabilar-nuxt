<template>
  <v-container class="fill-height about" fluid>
    <div class="d-flex flex-row ">
      <v-col cols="12">
        <v-row align="center">
          <v-col
            v-for="(item,i) in shoes"
            :key="i"
            cols="2"
            sm="2">
            <v-card>
              <nuxt-link :to="'/urun-detay/'+item.id">
                <v-img :src='item.img'></v-img>
              </nuxt-link>
              <v-row align="center" justify="center">
                <v-col cols="50">
                  <v-card-title class="ml-13 "> {{item.urunAd}}</v-card-title>
                  <v-card-text class="ml-15 font-weight-bold"> ₺{{item.fiyat}}</v-card-text>
                </v-col>
              </v-row>
            </v-card>
          </v-col>
        </v-row>
      </v-col>
    </div>
  </v-container>
</template>

<script>
  export default {
    name: 'Ayakkabilar',
    props: {
      shoes: {
        type: Array,
        default: [],
        required: false
      }
    },
  }
</script>
