<template>
  <footer>
    <div class="footer-container">
      <div class="flex">
        <div class="logo">
          <figure><img src="@/assets/LogoPositiveLife.png" alt="" /></figure>
        </div>
        <div class="contact">
          <h2>Contact Us</h2>
          <ul>
            <li>
              <i class="fa-brands fa-facebook"></i>
            </li>
            <li>
              <i class="fa-brands fa-instagram"></i>
            </li>
            <li>
              <i class="fa-brands fa-twitter"></i>
            </li>
            <li>
              <i class="fa-brands fa-youtube"></i>
            </li>
          </ul>
        </div>
      </div>
      <div class="copy">
        <!-- Copyright -->
        <p>© 2022 Todos los derechos reservados.</p>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  data() {
    return {};
  },
  name: "Footer",
  components: {},
};
</script>

<style lang="scss" scoped>
footer {
  width: 100%;
  color: #000;
  background-color: #f6f6f6;
}
.footer-container {
  display: flex;
  flex-direction: column;
  padding: 1rem;
}

.flex {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.logo {
  width: 25%;
  margin: 0;
  figure {
    width: 100%;
    margin: 0;
    img {
      width: 100%;
    }
  }
}

.copy {
  width: 50%;
  margin: 0 auto;
  p {
    margin: 0;
    font-size: 1rem;
    text-align: center;
  }
}

.contact {
  display: flex;
  flex-direction: column;
  width: 50%;
  h2 {
    margin: 0;
    margin-bottom: 1rem;
    text-align: center;
  }
  ul {
    list-style: none;
    display: flex;
    justify-content: space-between;
    li {
      padding: 0.5rem;
      border-radius: 5px;
      font-size: 1.5rem;
    }
    li:hover {
      background-color: #000;
      color: #fff;
      cursor: pointer;
      transition: all 0.3s ease-in-out;
    }
  }
}
/* TABLET */
@media screen and (min-width: 580px) {
  .logo {
    width: 20%;
  }

  .copy {
    width: 60%;
    p {
      font-size: 1rem;
    }
  }

  .contact {
    width: 60%;
    ul {
      justify-content: space-evenly;
      li:hover {
        color: #fff;
      }
    }
  }
}
/* PC */
@media screen and (min-width: 768px) {
  .logo {
    width: 15%;
  }

  .copy {
    width: 60%;
    p {
      font-size: 1rem;
    }
  }

  .contact {
    width: 60%;
    ul {
      justify-content: space-evenly;
      li:hover {
        color: #fff;
      }
    }
  }
}
/* LARGE SCREEN */
@media screen and (min-width: 990px) {
  .logo {
    width: 10%;
  }

  .contact {
    width: 40%;
    ul {
      justify-content: space-evenly;
      li:hover {
        color: #fff;
      }
    }
  }
}
</style>
