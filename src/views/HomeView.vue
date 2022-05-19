<template>
  <Nav id="reg"></Nav>
  <div  class="home-page">
    <section
      data-aos="fade-right"
      data-aos-easing="linear"
      data-aos-duration="500"
      class="welcome"
    >
      <h2 class="welcome-title">{{ title }}</h2>
      <div>
        <p class="welcom-text">This is your home, we support you</p>
        <p>Do you want to be part of our community?</p>
        <a class="welcom-link" href="http://">Sing Up</a>
      </div>
    </section>

    <div class="pretty-phrase">
      <p>Hey!</p>
      <p>This message is foy you❤️</p>
      <div class="phrase">
        <p>{{ message }}</p>
        <button @click="changePhrase">Do you want another?</button>
      </div>
    </div>
    <section
      data-aos="fade-up"
      data-aos-easing="linear"
      data-aos-duration="500"
      class="community"
    >
      <h2>Community</h2>
      <div class="community-container">
        <p>
          We are the largest community of help to take care of mental health.
        </p>
        <div class="community-items">
          <a href="https://discord.gg/BguAz4xt" class="item"
            ><i class="fa-brands fa-discord"></i
          ></a>
          <a href="https://discord.gg/BguAz4xt" class="item"
            ><i class="fa-brands fa-blogger"></i
          ></a>
          <a href="https://discord.gg/BguAz4xt" class="item"
            ><i class="fa-brands fa-facebook"></i
          ></a>
          <a href="https://discord.gg/BguAz4xt" class="item"
            ><i class="fa-brands fa-instagram"></i
          ></a>
        </div>
      </div>
    </section>
    <section
      data-aos="fade-left"
      data-aos-easing="linear"
      data-aos-duration="500"
      class="download"
    >
      <h2>Download our App</h2>
      <div class="download-container">
        <a href="https://discord.gg/BguAz4xt" class="item"
          ><i class="fa-brands fa-android"></i
        ></a>
        <a href="https://discord.gg/BguAz4xt" class="item"
          ><i class="fa-brands fa-apple"></i
        ></a>
        <a href="https://discord.gg/BguAz4xt" class="item"
          ><i class="fa-brands fa-windows"></i
        ></a>
      </div>
    </section>
  </div>
  <div data-aos="fade-up" class="reg-pag">
    <a class="reg-pag-link" href="#reg"
      ><i class="fa-solid fa-arrow-up"></i
    ></a>
  </div>
  <Footer></Footer>
</template>

<script>
import Nav from "@/components/Nav.vue";
import Footer from "@/components/Footer.vue";
import LoginView from "./LoginView.vue";
export default {
  data() {
    return {
      title: "Welcome to Positive Life",
      message: "We are here to help you :3.",
    };
  },
  methods: {
    changePhrase() {
      this.message = "Te amarrare a la cama y te daré duro contra el muro";
    },
  },
  name: "HomeView",
  components: {
    Nav,
    Footer,
    LoginView,
  },
};
</script>

<style lang="scss" scoped>
.home-page {
  width: 100%;
  height: auto;
  justify-content: center;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.welcome,
.community,
.download {
  width: 85%;
  height: 60vh;
  margin: 0 auto;
  margin-bottom: 2rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}
h2 {
  font-size: 2rem;
  color: #ff0c86;
  text-align: center;
  margin: 0;
  margin-bottom: 1rem;
}
div {
  color: #5a2767;
  text-align: center;
  a {
    display: block;
    color: #ff0c86;
    text-decoration: none;
    font-size: 1.2rem;
    padding: 10px;
    border-radius: 5px;
  }
  a:hover {
    background-color: #5a2767;
    color: #fff;
    transition: all 0.3s ease-in-out;
  }
}
.pretty-phrase {
  margin-top: 2rem;
}

.phrase {
  p {
    height: 3rem;
    width: 15rem;
    clip-path: polygon(
      0% 0%,
      100% 0%,
      100% 75%,
      75% 75%,
      75% 100%,
      50% 75%,
      0% 75%
    );
    background-color: #eed55c;
    text-align: center;
  }
}

.community {
  width: 85%;
  margin: 0 auto;
  margin-bottom: 2rem;
}

.community-items {
  display: flex;
  justify-content: space-evenly;
  align-items: center;
  margin-top: 2rem;
}

.download-container {
  display: flex;
  width: 100%;
  justify-content: space-evenly;
}

.reg-pag {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 1rem;
}

/* TABLET */
@media screen and (min-width: 580px) {
  .home-page {
    justify-content: center;
    display: flex;
    flex-direction: column;
  }

  .welcome,
  .community,
  .download {
    width: 90%;
    height: 60vh;
  }
  h2 {
    font-size: 1.5rem;
  }
  div {
    a {
      font-size: 1.3rem;
    }
  }

  .community-items a,
  .download-container a,
  .reg-pag-link {
    font-size: 1.8rem;
  }

  .phrase {
    p {
      width: 14rem;
    }
  }

  .download-container {
    display: flex;
    width: 100%;
    justify-content: space-evenly;
  }
}
/* PC */
@media screen and (min-width: 768px) {
  .welcome,
  .community,
  .download {
    width: 90%;
    height: 50vh;
  }
  h2 {
    font-size: 1.6rem;
  }
  div {
    a {
      font-size: 1.4rem;
    }
  }

  .community-items a,
  .download-container a,
  .reg-pag-link {
    font-size: 1.9rem;
  }
}
/* LARGE SCREEN */
@media screen and (min-width: 990px) {
  .home-page {
    justify-content: center;
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .welcome,
  .community,
  .download {
    width: 85%;
    height: 60vh;
    margin: 0 auto;
    margin-bottom: 2rem;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }
  h2 {
    font-size: 2rem;
    color: #ff0c86;
    text-align: center;
    margin: 0;
    margin-bottom: 1rem;
  }
  div {
    color: #5a2767;
    text-align: center;
    a {
      display: block;
      color: #ff0c86;
      text-decoration: none;
      font-size: 1.2rem;
      padding: 10px;
      border-radius: 5px;
    }
    a:hover {
      background-color: #5a2767;
      color: #fff;
      transition: all 0.3s ease-in-out;
    }
  }
  .pretty-phrase {
    margin-top: 2rem;
  }

  .phrase {
    p {
      height: 3rem;
      width: 15rem;
      clip-path: polygon(
        0% 0%,
        100% 0%,
        100% 75%,
        75% 75%,
        75% 100%,
        50% 75%,
        0% 75%
      );
      background-color: #eed55c;
      text-align: center;
    }
  }

  .welcome {
    justify-content: flex-start;
    align-items: flex-start;
    height: 30vh;
    margin-top: 1rem;
  }

  .community {
    justify-content: center;
    height: 30vh;
    align-items: center;
  }

  .download {
    justify-content: flex-end;
    height: 30vh;
    align-items: flex-end;
  }

  .pretty-phrase {
    display: none;
  }

  .community-items {
    display: flex;
    justify-content: space-evenly;
    align-items: center;
    margin-top: 2rem;
  }

  .download-container {
    justify-content: flex-end;
  }

  .download-container a {
    margin-right: 2rem;
  }
}
</style>
