<template>
  <div class="container">
    <div>
      <nav>
        <div class="navbar-inner">
          <h1 class="logo">
            <a href="/">enamel</a>
          </h1>
          <ul class="nav-links">
            <li>
              <!-- <a href="/#pricing">Pricing</a> -->
            </li>
          </ul>
          <div class="navbar-action">
            <a :href="`${url}/login`">Login</a>
          </div>
        </div>
      </nav>
      <div class="portfolio">
        <div class="hero">
          <!-- <div class="waves"></div> -->
          <div class="inner-content">
            <div class="info">
              <h1>No More Meetings</h1>
              <p>
                enamel is a project management software that both engineers <em>and</em> business people can use to collaborate efficiently.
              </p>
              <div class="signup">
                <a :href="url">Get started for free</a>                
              </div>
            </div>

            <div class="image-container">
              <img class="hero-image" src="../assets/img/UI.svg">
            </div>
          </div>

        </div>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  components: {
  },
  data() {
    return {
      url: 'https://app.enamel.tech'
    }
  }
}
</script>

<style lang="scss">
a {
  color: inherit;
  cursor: pointer;
  text-decoration: none;
}

.container {
  min-height: 100vh;
  // background: linear-gradient(35deg, #7967b1, #4A4090);

  /*display: flex;*/
/*  justify-content: center;
  align-items: center;
  text-align: center;*/
}

nav {
  position: absolute;
  z-index: 4;
  width: 100%;
  margin: 0 auto;
  max-width: 123rem;
  padding: 0 2rem;
}

.navbar-inner {
  // color: #fff;
  align-items: center;
  display: flex;
  font-size: 1.8rem;
  justify-content: space-between;
  padding: 40px 0;
}

h1, h2, h3, h4 {
  letter-spacing: -1px;
  margin: 0;
}

h1 {
  font-size: 32px;
  font-weight: 300;
  /*line-height: 72px;*/
}

.logo {
  font-family: 'Questrial', sans-serif;
  letter-spacing: 2px;
  margin-right: 15px;
  padding: 0;
  /*display: inline-block;*/
}

ul.nav-links {
  display: flex;
  flex: 1 1;
  list-style: none;
  margin: 0 1.6rem;
  padding: 0;
}

.nav-links, .navbar-action {
  font-size: 20px;
  opacity: .7;
  &:hover {
    opacity: 1;
  }
}

.portfolio {
  padding-top: 0;
  position: relative;
  z-index: 1;
}

.hero {
  position: relative;
  padding-top: 100px;
  // background: linear-gradient(35deg, #7967b1, #4A4090);
  // height: 800px;
  // height: 100%;
  // color: #fff;
  overflow: hidden;
}

.waves {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-image: url(/static/img/waves.svg);
  background-size: cover;
  background-repeat: no-repeat;
  z-index: 2;
}

.inner-content {
  display:flex;
  padding-top: 30px;
  // text-align: center;
  z-index: 99;
}

.inner-content > div {
  flex: 1 1;
}

.info {
  margin-left: 25px;
}

.image-container {
  // margin-left: 25px;
  margin: 25px;
  position: relative;
  height: 100%;
}

.hero-image {
  // height: 100%;
  // bottom: 0;
  // left: 50%;
  // margin-left: 4rem;
  // position: absolute;
  // top: 0;
}

.info > h1 {
  /*font-family: Georgia, serif;*/
  margin: 0 0 30px 0;
  font-size: 60px;
  letter-spacing: 1px;
}

.info > p {
  font-size: 22px;
  margin: auto;
  max-width: 700px;
  text-align: left;
  line-height: 35px;
  margin-bottom: 30px;
}

.signup > a {
  border: none;
  border-radius: 6px;
  color: #fff;
  cursor: pointer;
  display: inline-block;
  text-align: center;
  font-family: inherit;
  font-size: 1.3rem;
  font-weight: 600;
  // height: 40px;
  // line-height: 5.6rem;
  outline: none;
  padding: 13px 1.8rem;
  text-decoration: none;

  color: #fff;
  background-color: #48f;
  border-color: #409EFF;
}

@media screen and (max-width: 800px) {
  .info > h1 {
    font-size: 43px;
    text-align: center;
  }

  .info > p {
    font-size: 16px;
  }

  .hero {
    padding-right: 10%;
    padding-left: 10%;
  }

  .inner-content {
    display: initial;
  }

  .image-container {
    margin: 10% 0; 
  }

  .info {
    margin: 0;
  }

  .signup {
    // display: block;
    width: 220px;
    margin: auto;
  }

  .signup > a {
    width: 100%;
    font-size: 1rem;
  }
}

</style>

