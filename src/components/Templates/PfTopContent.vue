<template>
  <article class="content">
    <div class="hero">
      <div class="hero-bg"></div>
      <div class="profile-image">
        <img src="@/assets/profile_pic_400x400.jpg" />
      </div>
    </div>
    <div class="sns-links">
      <div class="tw">
        <a href="https://twitter.com/kill_in_sun/">
          <i class="fab fa-twitter fa-2x" />
        </a>
      </div>
      <div class="fb">
        <a href="https://www.facebook.com/Sefinannnnn">
          <i class="fab fa-facebook fa-2x" />
        </a>
      </div>
      <div class="gh">
        <a href="https://github.com/killinsun">
          <i class="fab fa-github fa-2x" />
        </a>
      </div>
    </div>
    <section>
      <h1>{{ msg }}</h1>
      <p>
        content content text text
      </p>
      <h2>Who am I?</h2>
      <p>
        hmm
      </p>
      <h2>Skills</h2>
      <h3>Languages</h3>
      <ul>
        <li>Japanese(Native)</li>
        <li>English</li>
      </ul>
      <h3>Programming Languages</h3>
      <ul>
        <li>JavaScript</li>
        <li>Kotlin(A little)</li>
      </ul>
      <h3>Frameworks</h3>
      <ul>
        <li>Vue.js</li>
        <li>Node.js</li>
      </ul>
    </section>
  </article>
</template>

<script>
export default {
  name: "PfTopContent",
  props: {
    msg: String
  }
};
</script>

<style scoped>
.hero {
  max-width: 1920px;
  width: 100%;
  position: relative;
  margin-bottom: 10%;
}
.hero-bg {
  /* 表示画像の高さ ÷ 表示画像の幅 × 100 */
  padding-top: 46.45%;
  background-size: 100% auto;
  background-image: url("../../assets/banner.jpg");
  background-repeat: no-repeat;
}

.profile-image {
  z-index: 2;
  position: absolute;
  top: 65%;
  left: 0;
  right: 0;
}
.profile-image > img {
  width: 25%;
  border-radius: 50%;
}
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
.sns-links > div {
  display: inline-block;
  margin-left: 0.5vw;
  margin-right: 0.5vw;
}
.sns-links > div > a {
  color: #2c3e50;
}
</style>
