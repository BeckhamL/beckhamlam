<template>
  <div class="container">
    <div>
      <p class="display-4 mb-0">Hi! I'm</p>
      <h1 class="display-1 font-weight-bold">Beckham Lam</h1>
      <p class="h3">> Front-End Developer</p>
    </div>
    <div>
      <h2 class="display-3 font-weight-bold">About</h2>
      <p class="lead">
        I grew up and lived in Toronto for 20 years until I went to McGill
        University in Montréal where graduated with a bachelor's in Computer
        Science/Economics. I currently work at Mobile Fringe where I code mostly
        with TypeScript, Vue.js, Nuxt.js, HTML and SCSS. In my free time, I love
        playing badminton and guitar and I post covers on
        <a
          href="https://www.youtube.com/channel/UCwJNVHtcUyQxJL32z6egXZQ/videos"
          target="_blank"
          >YouTube</a
        >!
      </p>
    </div>
    <div>
      <h2 class="display-3 font-weight-bold">Websites I've helped build</h2>
      <p class="lead">
        These are websites that I've had a major role in developing
      </p>
      <div class="row">
        <div v-for="(website, index) in websites" :key="index" class="col-lg-6">
          <website-card :website="website"></website-card>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import WebsiteCard from '../components/websiteCard.vue';
export default {
  components: {
    WebsiteCard
  },
  data() {
    return {
      websites: [
        {
          img_url: "/images/mazda.png",
          title: "Mazda Canada Test Drive",
          website: "https://www.mazda.ca/en/shopping-tools/book-a-test-drive/"
        }
      ]
    };
  }
};
</script>
