<template>
  <Nav></Nav>
  <article class="context">
    <h2>Contexto:</h2>
    <div class="context-one">
      <h3>¿Qué son las enfermedades mentales?</h3>
      <p>
        Las enfermedades o trastornos mentales son afecciones que impactan su
        pensamiento, sentimientos, estado de ánimo y comportamiento. Pueden ser
        ocasionales o duraderas (crónicas). Pueden afectar su capacidad de
        relacionarse con los demás y funcionar cada día.
      </p>
    </div>
    <div class="context-two">
      <h3>¿Cuáles son algunos tipos de enfermedades mentales?</h3>
      <p>
        Existen muchos tipos diferentes de trastornos mentales. Algunos comunes
        incluyen:
      </p>
      <ul>
        <li>
          Trastornos de ansiedad, incluyendo trastorno de pánico, trastorno
          obsesivo-compulsivo y fobias
        </li>
        <li>
          Depresión, trastorno bipolar y otros trastornos del estado de ánimo
        </li>
        <li>Trastornos de la alimentación</li>
        <li>Trastornos de la personalidad</li>
        <li>Trastorno de estrés post-traumático</li>
        <li>incluyendo</li>
      </ul>
      <a
        class="context-link"
        href="https://medlineplus.gov/spanish/mentaldisorders.html"
        target="_blank"
        rel="noopener noreferrer"
        >More info</a
      >
    </div>
    <div class="context-three">
      <h3>Motivación</h3>
      <p>
        Según las últimas estimaciones disponibles, se calcula que más de 1 de
        cada 7 adolescentes de 10 a 19 años sufre un trastorno mental
        diagnosticado en todo el mundo. Casi 46.000 adolescentes se suicidan
        cada año, una de las cinco principales causas de muerte para este grupo
        de edad. Al mismo tiempo, sigue habiendo grandes diferencias entre las
        necesidades relacionadas con la salud mental y la financiación destinada
        a esta cuestión. El informe concluye que solamente alrededor del 2% de
        los presupuestos de salud de los gobiernos se destinan a la salud mental
        en todo el mundo.
      </p>
      <p>
        “Los últimos 18 meses han sido muy largos para todos nosotros,
        especialmente para los niños y niñas. Debido a los confinamientos
        nacionales y a las restricciones de movimiento relacionadas con la
        pandemia, los niños han perdido un tiempo valioso de sus vidas lejos de
        la familia, los amigos, las aulas y los lugares de recreo, que son muy
        importantes durante la infancia”, dijo Henrietta Fore, Directora
        Ejecutiva de UNICEF. “Las consecuencias de la pandemia tienen un gran
        alcance, pero son sólo la punta del iceberg. Incluso antes de la
        pandemia ya había demasiados niños abrumados por el peso de una serie de
        problemas de salud mental a los que no se les había prestado atención.
        Los gobiernos están invirtiendo muy poco para atender estas necesidades
        esenciales. No se está dando suficiente importancia a la relación entre
        la salud mental y las consecuencias que se producen más adelante en la
        vida”.
      </p>
      <p>
        Todo esto nos llevo a crear esta iniciativa en pro de mitigar un poco
        las consecuencias que trajo el paso del covid-19 en nuestras vidas. Por
        eso llega, Positive Life
      </p>
      <a
        class="context-link"
        target="_blank"
        href="https://www.unicef.org/es/comunicados-prensa/efectos-nocivos-covid19-salud-mental-ninos-ninas-jovenes-punta-iceberg?gclid=Cj0KCQjwspKUBhCvARIsAB2IYuvptzFtMR5dbZ8-7VSn2pTNyP0Qiihyo90IfyEh23OD2UTr62Ly5ToaAm8nEALw_wcB"
        >More Info</a
      >
    </div>
  </article>
  <article class="work-team">
    <h2>Work Team</h2>
    <div class="work-team-description">
      <p>
        El equipo de Positive Life está conformado por un grupo de personas que
        se dedicaron a la investigación y desarrollo de esta App web.
      </p>
      <p>El equipo está conformado por:</p>
    </div>
    <Card></Card>
  </article>
  <Footer></Footer>
</template>

<script>
import Nav from "@/components/Nav.vue";
import Footer from "@/components/Footer.vue";
import Home from "@/components/Home.vue";
import Card from "@/components/Card.vue";
export default {
  name: "AboutView",
  components: {
    Nav,
    Footer,
    Home,
    Card,
  },
};
</script>

<style lang="scss" scoped>
.context {
  display: flex;
  flex-wrap: wrap;
  width: 90%;
  margin: 0 auto;
  h2 {
    font-size: 1.7rem;
    margin: 2rem 0;
    color: var(--morado);
  }
}

h2,
h3 {
  color: var(--morado);
}
p {
  font-size: 1.2rem;
  line-height: 2rem;
  margin: 1rem 0;
  text-align: justify;
  color: var(--rosado);
}

li {
  font-size: 1.1rem;
  line-height: 1.2rem;
  margin: 1rem 0;
  color: var(--rosado);
}

.work-team {
  width: 90%;
  margin: 0 auto;
}

a {
  color: var(--morado);
  text-decoration: none;
  display: inline-block;
  vertical-align: middle;
  transform: translateZ(0);
  box-shadow: 0 0 1px rgba(0, 0, 0, 0);
  backface-visibility: hidden;
  -moz-osx-font-smoothing: grayscale;
  transition-duration: 0.3s;
  transition-property: transform;
}

a:hover {
  transform: scale(1.2);
}
/* TABLET */
@media screen and (min-width: 580px) {
  .context {
    h2 {
      font-size: 1.6rem;
    }
  }
  p {
    font-size: 1.1rem;
    line-height: 1.8rem;
  }

  li {
    font-size: 1rem;
    line-height: 1rem;
  }
}
/* PC */
@media screen and (min-width: 768px) {
  .context {
    h2 {
      font-size: 1.5rem;
    }
  }
  p {
    font-size: 1rem;
    line-height: 1.5rem;
  }

  li {
    font-size: 0.9rem;
    line-height: 0.8rem;
  }
}
/* LARGE SCREEN */
@media screen and (min-width: 990px) {
}
</style>
