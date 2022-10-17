<template>
  <div>
    <div>
      <div style="width: 100%; opacity: 0.3">
        <video
          src="https://firebasestorage.googleapis.com/v0/b/treetanium-world.appspot.com/o/yeansite%2Fvideo%2Fdev_9.mp4?alt=media&token=ff9e4f5b-e37e-4959-a71b-8647b7c72af5"
          ref="introVideo"
          autoplay
          loop
        ></video>
      </div>
      <v-container fluid class="spacing-top-50">
        <v-row class="text-left">
          <v-col class="hidden-mobile" md="2"></v-col>
          <v-col xs="12" sm="3" md="3" lg="3" class="spacing-row-100x100">
            <div
              style="
                font-size: 100px;
                font-family: 'Times New Roman', Times, serif;
              "
            >
              _ _
            </div>
            <div class="text-h2 mb-10">Design & ergonomics</div>
            <div class="text-h6 font-weight-regular">
              In my work, I try to find the right balance between form and
              function. From technical drawings, all the way to the photographic
              renders, and the actual representations of my work as a designer,
              my philosophy is that of simplicity. At the same time, my style is
              distinctly mine – uncluttered, with clean shapes and modern
              space-saving solutions.
            </div>
          </v-col>

          <v-col xs="12" sm="12" md="5">
            <v-img
              class="simply-imagen my-3"
              src="https://firebasestorage.googleapis.com/v0/b/treetanium-world.appspot.com/o/yeansite%2Fvideo%2Fdev_2.jpg?alt=media&token=12da3ce1-7c62-4c1d-85b3-394a9f970b36"
            />
          </v-col>
          <v-col col="2"></v-col>
        </v-row>
        <v-row class="text-center"
          ><div class="spacing-title-300">
            <v-col cols="12 mt-m-5">
              <div class="text-h2 mt-m-5">“A sample of my work”</div>
            </v-col>
          </div>
        </v-row>
      </v-container>
    </div>
    <v-container>
      <v-row class="spacing-row-mobile-100x100">
        <v-col
          v-for="skill in skills"
          :key="skill.title"
          sm="6"
          md="3"
          xs="12"
          lg="3"
          class="mt-15"
        >
          <v-card>
            <v-img
              :src="skill.img"
              class="white--text align-end"
              gradient="to bottom, rgba(0,0,0,.1), rgba(0,0,0,.5)"
              height="200px"
            >
              <v-card-title v-text="skill.title"></v-card-title>
              <v-card-text v-text="skill.text"></v-card-text>
            </v-img>

            <v-card-actions>
              <v-spacer></v-spacer>

              <v-btn icon :href="skill.src">
                <v-icon>mdi-web</v-icon>
              </v-btn>

              <v-btn icon>
                <v-icon>mdi-heart</v-icon>
              </v-btn>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
    <div style="background-color: rgb(58 69 90)">
      <v-container>
        <v-row class="text-left">
          <v-col class="hidden-mobile" md="2"></v-col>
          <v-col xs="12" sm="3" md="3" lg="3" class="spacing-row-100x100">
            <div
              class="white--text"
              style="
                font-size: 100px;
                font-family: 'Times New Roman', Times, serif;
              "
            >
              _ _
            </div>
            <div class="text-h2 mb-10 white--text">
              My experience as a freelancer
            </div>
            <div class="text-h6 font-weight-regular font-italic white--text">
              In my work, I try to find the right balance between form and
              function. From technical drawings, all the way to the photographic
              renders, and the actual representations of my work as a designer,
              my philosophy is that of simplicity. At the same time, my style is
              distinctly mine – uncluttered, with clean shapes and modern
              space-saving solutions.
            </div>
          </v-col>

          <v-col xs="12" sm="12" md="5">
            <v-img
              class="simply-imagen my-3"
              src="https://firebasestorage.googleapis.com/v0/b/treetanium-world.appspot.com/o/yeansite%2Fvideo%2Fdev_1.jpg?alt=media&token=2f0a5fbf-c6dd-4330-8c21-ad25fa5fe9c6"
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
  name: "fragment1",
  data: () => ({
    skills: [
      {
        title: "Tokenbase",
        src: "https://www.tokenbase.live",
        img: "https://firebasestorage.googleapis.com/v0/b/treetanium-world.appspot.com/o/yeansite%2Fdev_tk.png?alt=media&token=18fcbee1-78f1-4784-a637-7d4c03e10356",
      },
      {
        title: "Treetanium",
        src: "https://www.treetanium.com",
        text: "Sitio web para la gestion de un proyecto relacionado al medio ambiente",
        img: "https://firebasestorage.googleapis.com/v0/b/treetanium-world.appspot.com/o/yeansite%2Fdev_ttr.png?alt=media&token=8ce34ce3-b1bd-404b-a300-cecccc9d1aff",
      },
      {
        title: "Coinworld",
        img: "https://firebasestorage.googleapis.com/v0/b/treetanium-world.appspot.com/o/yeansite%2Fdev_cw.png?alt=media&token=e6ae5745-e8fc-415b-b656-574e0899fa18",
        src: "https://coinworld-la.web.app/",
        text: "App-web para la compra y venta de fichas de juegos, entre usuarios p2p",
      },
      {
        title: "Github",
        src: "https://github.com/Yean-ZX0",
        text: "My Public repositories",
        img: "https://firebasestorage.googleapis.com/v0/b/treetanium-world.appspot.com/o/yeansite%2Fdev_git.jpg?alt=media&token=6f608826-255d-4d05-848f-c8351150e03d",
      },
      {
        title: "CRM IChruch",
        src: "https://ichurch-f430f.web.app/",
        text: "Software para gestion de iglesias",
        img: "https://firebasestorage.googleapis.com/v0/b/treetanium-world.appspot.com/o/yeansite%2Fdev_churc.png?alt=media&token=2fad78d6-cc8e-477e-848e-c2e9431439b6",
      },

      {
        title: "Blockchain",
        img: "https://firebasestorage.googleapis.com/v0/b/treetanium-world.appspot.com/o/yeansite%2Fdev_block.png?alt=media&token=9c9319c9-5924-45a5-8873-9c3e7262bd86",
        src: "https://bscscan.com/token/0x300ad0d9058a1ccadbc3d60e36400c33d5b6ba7a#readContract",
        text: "This contract is a test deploy for me",
      },
    ],
  }),
};
</script>
