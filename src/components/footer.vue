<template>
  <v-container>
    <v-row class="text-left spacing-row-100x250">
      <v-col class="hidden-mobile" md="1"></v-col>
      <v-col cols="12" xs="12" sm="12"  md="7" >
        <div class="text-h2">Follow me in Social Media</div>
        <div class="mt-5">
          <v-row
            ><v-col cols="2">
              <v-btn text target="_blank" href=""
                ><v-icon x-large>mdi-github</v-icon></v-btn
              >
            </v-col>
            <v-col cols="2">
              <v-btn text target="_blank" href=""
                ><v-icon x-large>mdi-twitter</v-icon></v-btn
              >
            </v-col>
            <v-col cols="2">
              <v-btn text target="_blank" href=""
                ><v-icon x-large>mdi-linkedin</v-icon></v-btn
              >
            </v-col>
          </v-row>
        </div>
      </v-col>
      <v-col cols="12" xs="12" sm="12" md="2" class="mt-m-15">
        <div class="text-h4 mb-10">
          <v-icon x-large>mdi-account-box</v-icon> Contacts
        </div>
        <div class="text-h6">
          <v-icon>mdi-cellphone</v-icon> zzzzzzzzzzzz
        </div>
        <div class="text-h6">
          <v-icon>mdi-email</v-icon> zzzzzzzzzzzzz
        </div>
      </v-col>
      <v-col class="hidden-mobile" cols="1"></v-col>
    </v-row>
  </v-container>
</template>
