<template>
  <nav class="global-nav">
    <div class="gnav-inline-blocks">
      <div class="gnav-hamburger-menu">
        <i class="fas fa-bars fa-2x"></i>
      </div>
      <div class="gnav-site-title">
        <router-link to="/" wovn-ignore>
          {{ title }}
        </router-link>
      </div>
      <div id="nav">
        <router-link to="/">Home</router-link> |
        <router-link to="/about">About</router-link> |
        <router-link to="/Media">Media</router-link>
      </div>
    </div>
  </nav>
</template>

<script>
export default {
  data: function() {
    return {
      title: "KILLINSUN.COM"
    };
  }
};
</script>
<style scoped>
nav.global-nav {
  width: 100%;
}

div.gnav-inline-blocks > div {
  display: inline-block;
}

div.gnav-inline-blocks > .gnav-hamburger-menu {
  padding-right: 2vw;
}

div.gnav-inline-blocks > .gnav-site-title {
  font-weight: bold;
  padding-right: 60vw;
  font-size: 2vw;
}
div.gnav-inline-blocks > .gnav-site-title a {
  color: #2c3e50;
  text-decoration: none;
}

.global-nav {
  padding-top: 3vh;
  padding-bottom: 3vh;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
