<template>
  <Gallery v-bind:projects="projects" />
</template>

<script>
// @ is an alias to /src
import Gallery from "@/components/Gallery.vue";

export default {
  name: "home",
  components: {
    Gallery
  },
  data() {
    return {
      projects: [
        {
          url: "https://live.staticflickr.com/65535/52125022752_3e62e61db6_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/52126048568_ba1df5b28a_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/52125788269_46d5f84509_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/51247021420_003d40ee92_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/51245967956_081fcbb895_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/51245954166_f891138c31_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/51156230492_462fc3e305_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/51156230707_a21c96f298_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/51157682734_9c457b3b51_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/51157565904_7c1ffc8c16_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/51156782031_c3de193a27_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/51157565109_bd524424ad_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/51157016803_e42ac46c0a_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/51157886680_290d87c31a_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/51157564134_4534a182f4_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/51156116002_870978276b_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/51156781736_d55aa223fb_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/51157016008_af13afee41_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/51157887065_27cc51d869_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/51157016528_7abb022011_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/51157564779_f6673692f8_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/51156116842_bee77c0d78_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/51156782531_6c418a7146_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/51156117007_913e9fe418_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/51156116232_1919f3249a_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/51157887465_9b3d1d697b_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/51157887440_5c50fac79d_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/51156781936_b9bca5acf5_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/51156782176_8cacb7540d_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/51157886855_3b8540ad0d_h.jpg",
          name: "",
          description: ""
        },
      ]
    };
  }
};
</script>
