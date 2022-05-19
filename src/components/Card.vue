<template>
  <div class="card-container">
    <div data-aos="zoom-in-right" class="card">
      <figure>
        <img src="@/assets/StevenH.jpg" alt="Desarrollador" />
      </figure>
      <div data-aos="fade-down" class="card-header">
        <h3>{{ name[0] }}</h3>
      </div>
      <div data-aos="fade-right"  class="card-body">
        <p>Desarrollador Front-End.</p>
        <p>Aunar</p>
      </div>
    </div>
    <div data-aos="zoom-in" class="card">
      <figure>
        <img src="@/assets/tomas.jpeg" alt="Desarrollador" />
      </figure>
      <div data-aos="fade-down" class="card-header">
        <h3>{{ name[1] }}</h3>
      </div>
      <div data-aos="fade-right" class="card-body">
        <p>Desarrollador Front-End.</p>
        <p>Aunar</p>
      </div>
    </div>
    <div data-aos="zoom-in-left" class="card">
      <figure>
        <img src="@/assets/StevenQ.jpeg" alt="Desarrollador" />
      </figure>
      <div data-aos="fade-down" class="card-header">
        <h3>{{ name[2] }}</h3>
      </div>
      <div data-aos="fade-right" class="card-body">
        <p>Desarrollador Back-End.</p>
        <p>Aunar</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      name: ["Steven", "Tomas", "Steven "],
    };
  },
  name: "Card",
  components: {},
};
</script>

<style lang="scss" scoped>
.card-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 0 auto;
}

.card {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 50%;
  text-align: center;
  padding: 1rem;
  figure {
    width: 100%;
    margin: 0;
    img {
      width: 100%;
      border-radius: 50%;
    }
  }
  h3 {
    margin: 0;
    font-size: 1.7rem;
    margin: 1rem 0;
    color: var(--morado);
  }
  p {
    margin: 0;
    font-size: 1.2rem;
    line-height: 2rem;
    color: var(--rosado);
  }
}

/* TABLET */
@media screen and (min-width: 580px) {
  .card-container {
    flex-direction: row;
    align-items: center;
  }

  .card {
    width: 45%;
    text-align: center;
    p {
      font-size: 1.2rem;
      line-height: 1.5rem;
    }
  }
}
/* PC */
@media screen and (min-width: 768px) {
  .card {
    width: 20%;
    margin: 0 auto;
    figure {
      width: 80%;
      margin: 0;
      img {
        width: 100%;
        border-radius: 50%;
      }
    }
  }
}
/* LARGE SCREEN */
@media screen and (min-width: 990px) {
}
</style>
