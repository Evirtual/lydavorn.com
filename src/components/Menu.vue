<template>
  <div>
    <router-link to="/" class="logo">
      <img alt="vorn logo" src="../assets/vorn.svg" />
    </router-link>
    <div class="nav">
      <router-link to="/" class="nav-home"></router-link>
      <router-link to="/crochet" class="nav-corchet"></router-link>
      <router-link to="/about" class="nav-about"></router-link>
    </div>
  </div>
</template>

<script>
export default {
  name: "SideMenu",
  data: function() {
    return {
      isActive: false
    };
  },
  methods: {
    makeActive: function() {
      this.isActive = true;
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.logo {
  position: relative;
  display: inline-block;
  height: 50px;
  margin: 20px;
  @media only screen and (min-width: 768px) {
    position: fixed;
    top: 0;
    left: 0;
    height: 100px;
    margin: 3em;
  }
  img {
    height: 100%;
  }
}
.nav {
  position: absolute;
  top: 25px;
  right: 20px;
  @media only screen and (min-width: 768px) {
    position: fixed;
    top: auto;
    bottom: 2rem;
    left: 2rem;
    margin: 0;
    width: 90px;
  }
  @media only screen and (min-width: 1024px) {
    bottom: 3rem;
    left: 3rem;
    width: 55px;
  }
  a {
    display: inline-block;
    width: 40px;
    margin-left: 15px;
    height: 40px;
    background-size: 15px;
    background-position: center;
    background-repeat: no-repeat;
    opacity: 0.85;
    border: 1px solid white;
    transition: opacity 0.25s ease-in-out, background 0.25s ease-in-out, box-shadow 0.25s ease-in-out;
    border-radius: 50%;
    @media only screen and (min-width: 768px) {
      margin: 5px;
    }
    @media only screen and (min-width: 1024px) {
      display: block;
      width: 55px;
      height: 55px;
      background-size: 32px;
      margin: auto;
      margin-top: 20px;
    }
    &:hover {
      opacity: 1;
    }
    &.router-link-exact-active {
      opacity: 1;
      box-shadow: 0 0 8px rgba(0, 0, 0, 0.2);
    }
  }
}
.nav-home {
  background-position: 5px center !important;
  background-image: url("../assets/picture.svg");
  @media only screen and (min-width: 768px) {
    background-position: 9px center !important;
  }
}
.nav-corchet {
  background-image: url("../assets/yarn.svg");
}
.nav-about {
  background-image: url("../assets/woman.svg");
}
</style>
