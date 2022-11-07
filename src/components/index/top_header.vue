<template>
  <div>
    <div>
      <div class="video-background">
        <video
          src="https://firebasestorage.googleapis.com/v0/b/treetanium-world.appspot.com/o/yeansite%2Fvideo%2Fdev_6.mp4?alt=media&token=22bdab17-a0d7-46bf-8730-451d396e8e66"
          ref="introVideo"
          autoplay
          loop
        ></video>
      </div>
      <v-container fluid class="container-absoluted">
        <v-row class="text-center">
          <v-col cols="12">
            <div
              class=""
              style="
                font-family: 'Century Gothic', CenturyGothic, AppleGothic, sans-serif;
                font-size: 105px;
              "
            >
              Example name
            </div>
            <div
              class="text-h5 mb-15"
              style="font-family: 'Consolas', monaco, monospace"
            >
              Example Job
            </div>
            <v-img
              :src="require('../../assets/logo.svg')"
              class="my-3"
              contain
              height="120"
            />
          </v-col>
        </v-row>
        <v-row class="mt-10">
          <v-col
            v-for="skill in skills"
            :key="skill.title"
             sm="6" md="4" xs="12" lg="2"
            class="mt-15"
          >
            <v-card>
              <v-img
                :src="skill.img"
                class="white--text align-end"
                gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.2)"
                height="160px"
              >
                <v-card-title v-text="skill.title"></v-card-title>
              </v-img>

              <v-card-actions>
                <v-spacer></v-spacer>

                <v-btn icon>
                  <v-icon>mdi-heart</v-icon>
                </v-btn>

                <v-btn icon>
                  <v-icon>mdi-share-variant</v-icon>
                </v-btn>
              </v-card-actions>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </div>
    <v-container>
      <v-row class="text-center">
        <v-col cols="12" style="padding-top: 350px; padding-bottom: 250px">
          <div class="text-h2">“Degins website is my pasion”</div>
        </v-col>
      </v-row>
    </v-container>
    <div style="background-color: rgb(20 21 23)">
      <v-container>
        <v-row class="text-left">
          <v-col class="hidden-mobile" md="2" ></v-col>
          <v-col xs="12" sm="3" md="3" lg="3" style="padding-top: 100px; padding-bottom: 100px">
            <div
              class="white--text"
              style="
                font-size: 100px;
                font-family: 'Times New Roman', Times, serif;
              "
            >
              _ _
            </div>
            <div class="text-h2 mb-10 white--text">My Philosophy</div>
            <div class="text-h6 font-weight-regular font-italic white--text">
              In my work, I try to find the right balance between form and
              function. From technical drawings, all the way to the photographic
              renders, and the actual representations of my work as a designer,
              my philosophy is that of simplicity. At the same time, my style is
              distinctly mine – uncluttered, with clean shapes and modern
              space-saving solutions.
            </div>
          </v-col>

          <v-col xs="12" sm="12" md="5" class="pt-15">
            <v-img
              src="https://firebasestorage.googleapis.com/v0/b/treetanium-world.appspot.com/o/yeansite%2Fvideo%2Fdev_1.jpg?alt=media&token=2f0a5fbf-c6dd-4330-8c21-ad25fa5fe9c6"
              class="my-3"
              height="600"
              style="border-radius: 30px"
            />
          </v-col>
          <v-col col="2"></v-col>
        </v-row>
      </v-container>
    </div>
  </div>
</template>
<script>
export default {
  name: "top-header",
  data: () => ({
    skills: [
      { title: "ReactJS" , img:'https://firebasestorage.googleapis.com/v0/b/treetanium-world.appspot.com/o/yeansite%2Fdev_react.png?alt=media&token=b228f992-7532-4cae-b68c-9199c043402c'},
      { title: "VueJS", img:'https://firebasestorage.googleapis.com/v0/b/treetanium-world.appspot.com/o/yeansite%2Fdev_vue.png?alt=media&token=3df54cfe-840c-4c20-b708-08b5c7d53b31' },
      { title: "ExpressJS", img:'https://firebasestorage.googleapis.com/v0/b/treetanium-world.appspot.com/o/yeansite%2Fdev_ex.png?alt=media&token=1882141b-5312-47c6-b7b1-2bea1f5a67b4' },
      { title: "Nodejs", img:'https://firebasestorage.googleapis.com/v0/b/treetanium-world.appspot.com/o/yeansite%2Fdev_node.png?alt=media&token=d04184e4-7171-4143-8e03-4598de4971f4' },
      { title: "MongoDB", img:'https://firebasestorage.googleapis.com/v0/b/treetanium-world.appspot.com/o/yeansite%2Fdev_4.png?alt=media&token=392a7f15-6c30-4246-9f8b-f7d5deaa659f' },
      { title: "Blockchain", img:'https://firebasestorage.googleapis.com/v0/b/treetanium-world.appspot.com/o/yeansite%2Fdev_block.png?alt=media&token=9c9319c9-5924-45a5-8873-9c3e7262bd86' },
    ],
  }),
  mounted() {
    this.$refs.introVideo.play;
  },
};
</script>
