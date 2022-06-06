<template>
  <Gallery v-bind:projects="projects" />
</template>

<script>
// @ is an alias to /src
import Gallery from "@/components/Gallery.vue";

export default {
  name: "crochet",
  components: {
    Gallery
  },
  data() {
    return {
      projects: [
        {
          url: "https://live.staticflickr.com/65535/52125542621_5fb322230a_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/52125790174_b577278411_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/52124524747_962d4e257d_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/52126050330_765785091c_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/52125578733_97e48e4676_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/52126051545_ccc668a867_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/52125792149_118e348139_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/52124526367_6be2250921_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/52126052285_f8b6bbbd70_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/52125545911_3be7db3c6c_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/52125580508_27378ede82_h.jpg",
          name: "",
          description: ""
        },
        {
          url: "https://live.staticflickr.com/65535/52124528652_90f1aa0f11_h.jpg",
          name: "",
          description: ""
        },
        
      ]
    };
  }
};
</script>
