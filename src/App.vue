<template>
  <div>
    <div class="noticias">
      <div class="container">
        <!--Seccion superior-->

        <!--Seccion de noticias-->
        <div id="news">
          <componente-noticias></componente-noticias>
        </div>
      </div>
    </div>

    <div class="container mt-5">
      <!--Seccion de equipos-->
      <div id="team" class="card-deck">
        <team-card
          v-for="(member, index) of members"
          :key="index"
          :member="member"
        ></team-card>
      </div>
    </div>

    <div class="bg-dark">
      <div class="container ">
        <!--Seccion Footer-->
        <div id="footer">
          <footer-section></footer-section>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ComponenteNoticias from "./components/ComponenteNoticias.vue";
import FooterSection from "./components/FooterSection.vue";
import TeamCard from "./components/TeamCard.vue";
export default {
  name: "App",
  components: {
    ComponenteNoticias,
    TeamCard,
    FooterSection,
  },
  data() {
    return {
      members: [
        {
          codigo: "1",
          nombre: "Ivan Aldana",
          descripcion:
            "Eterno interesado en la tecnología y los descubrimientos científicos. Convencido de que el cielo ya no es el lìmite",
          rol: "Desarrollador FrontEnd",
          image: "./images/IvanCAldana.jpg",
        },
        {
          codigo: "2",
          nombre: "Eduardo Gallo",
          descripcion:
            "Entusiasta de la programación y de aprender cosas nuevas, me encantan los videojuegos, el anime.",
          rol: "Desarrollador FullStack",
          image: "./images/Gallo.jpg",
        },
        {
          codigo: "3",
          nombre: "Jose Bohorquez",
          descripcion:
            "Apasionado por la pedadogía, el cine y de como la palabra Lorem se convierte en la retahíla de letras en Latín (?) en el VSCode",
          rol: "Desarrollador BackEnd",
          image: "./images/JoseBohorquez.jpg",
        },
      ],
    };
  },
};
</script>

<style scoped>
.noticias {
  background: url(https://cdn.pixabay.com/photo/2018/10/11/19/04/sketch-3740576_1280.jpg)
    no-repeat fixed center;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
  height: 100%;
  width: 100%;
  text-align: center;
}

</style>

