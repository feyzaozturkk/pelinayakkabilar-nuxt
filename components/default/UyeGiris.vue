<template>
  <v-container class="fill-height about" fluid>
    <v-row align="center" justify="center">
      <v-col cols="12" sm="12" align="center">
        <v-card class="elevation-12" color="#FFFFF" style="padding: 10px;padding-bottom: 50px" width="500px">
          <div>
            <h1 class="black--text text-sm-left ml-5 mb-5 mt-5">Üye Girişi</h1>
            <v-text-field dense class="rounded-0 ml-5 mr-5" outlined label="E-posta"></v-text-field>
            <v-text-field dense class="rounded-0 ml-5 mr-5" type="password" outlined label="Şifre"></v-text-field>
            <v-btn class="rounded-0" style="background-color:#FF80AB; color:white" width="450px">Giriş Yap</v-btn>
            <div class="d-flex flex-row ">
              <v-checkbox class="ml-10" label="Beni Hatırla"></v-checkbox>
              <label style="width:150px"></label>

              <v-btn small class="font-weight-light text-decoration-underline mt-5" text> Şifremi Unuttum</v-btn>
            </div>
           <nuxt-link to="/">
             <v-btn class="rounded-0" style="background-color:#FF80AB; color:white" width="450px">Üyeliksiz Devam Et</v-btn>
           </nuxt-link>
          </div>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
  export default {
    name: 'UyeGiris'
  }
</script>
