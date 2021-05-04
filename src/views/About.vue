<template>
  <div class="about">
    <div v-for="profile in profiles" :key="profile.id">
      <div class="about-info">
        <h3>Story about me</h3>
        <p>My name is Lyda. I am from a big family with one brother and seven sisters. Until I was twelve years old, I lived in a province of Cambodia. After my parents split, I chose to go with my mom to Phnom Penh, where life was not easy but better than listen to my parents arguing.</p>
        <p>Phnom Penh is the capital city of Cambodia and still developing - a lot of buildings and businesses rising with a lot of consumption happening. So we have a lot of trash around the city. Once my mom came to the city and started to work as a scavenger, and I joined to help her so we could survive in this busy city.</p>
        <p>Before coming to the city, I didn't have any education and wanted to learn English because my dream was to be an interpreter so, I joined an organization where they teach kids, give them a place to stay and food for free. From that moment, I stopped scavenging and focused on studying. But I still wanted to support my mom and started to work as a part-time waitress. I was the oldest student there and felt embarrassed, but my wish to be a smart girl was stronger than shame. I stayed in the organization for ten years and met more kids like me - it helped me feel better about myself.</p>
        <p>After all the struggle, I am so happy that I never gave up and keep learning to this day.</p>
      </div>
      <div class="about-contacts">
        <h4>Contact Me</h4>
        <p>{{ profile.name }}</p>
        <p>{{ profile.phone }}</p>
        <p>
          <a
            :href="`mailto:${profile.email}`"
            target="_blank"
            rel="noopener noreferrer"
            >{{ profile.email }}</a
          >
        </p>
      </div>
      <div class="about-social">
        <a
          v-for="s in socials"
          :key="`${s.id}`"
          :href="`${s.url}`"
          target="_blank"
          :style="`color:${s.color};`"
          rel="noopener noreferrer"
          >{{ s.name }}<span>|</span></a
        >
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "About",
  data() {
    return {
      profiles: [
        {
          name: "Lyda Vorn",
          phone: "+855 969 412859",
          email: "contact@lydavorn.com",
        }
      ],
      socials: [
        {
          url: "https://www.linkedin.com/in/vorn-lyda/",
          name: "LinkedIn",
          color: "#007bb5"
        },
        {
          url: "https://www.facebook.com/vorn.lyda.kh",
          name: "Facebook",
          color: "#3b5998"
        },
        {
          url: "https://www.instagram.com/lyda_vorn/",
          name: "Instagram",
          color: "#e4405f"
        }
      ]
    };
  }
};
</script>

<style lang="scss">
.about {
  margin-bottom: 20px;
  max-width: 550px;
  padding: 1.5rem;
  background: rgba(255, 255, 255, 0.85);
  color: black;
  box-shadow: 0 0 15px rgba(0, 0, 0, 0.25);
  font-size: 0.8em;
  @media only screen and (min-width: 768px) {
    font-size: 1em;
    margin-bottom: 0;
  }
  h3 {
    font-size: 2.5em;
    margin-top: 0;
  }
  h4 {
    font-size: 1.1em;
    margin-top: 30px;
    font-weight: 500;
  }
  p {
    font-size: 1.15em;
    line-height: 1.25;
  }
  .about-contacts {
    p {
      margin-top: 0;
      margin-bottom: 5px;
    }
    a {
      color: black;
      text-decoration: none;
      &:hover {
        text-decoration: underline;
      }
    }
  }
  .about-skills {
    span {
      display: inline-block;
      font-size: 1.15em;
      margin-right: 5px;
      &:last-child {
        i {
          display: none;
        }
      }
    }
  }
  .about-social {
    margin-top: 30px;
    a {
      font-weight: 400;
      display: inline-block;
      margin-bottom: 5px;
      margin-right: 10px;
      text-decoration: none;
      &:hover {
        text-decoration: underline;
      }
      span {
        margin-left: 10px;
        font-style: normal;
        color: black;
      }
      &:last-child {
        span {
          display: none;
        }
      }
    }
  }
}
</style>
