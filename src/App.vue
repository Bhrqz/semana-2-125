<template>
  <div id="app" class="integranteContainer mt-4 d-flex ml-2 justify-content-around" width="100%">
    <team-card class="integrante mt-3" 
      v-bind:member="{ 
        nombre: 'Ivan Aldana',
        descripcion: 'Eterno interesado en la tecnología y los descubrimientos científicos. Convencido de que el cielo ya no es el lìmite',
        codigo: '1',
        image: 'IvanCAldana.jpg',
        rol: 'Desarrollador FrontEnd'
        }"
        ></team-card>
    
    <team-card class="integrante mt-3" 
      v-bind:member="{ 
        nombre: 'Eduardo Gallo',
        descripcion: 'Entusiasta de la programación y de aprender cosas nuevas, me encantan los videojuegos, el anime y los dibujos animados.',
        codigo: '2',
        image: 'Gallo.jpg',
        rol: 'Desarrollador FullStack'
        }"
        ></team-card>
    
    <team-card class="integrante mt-3" 
      v-bind:member="{ 
        nombre: 'Jose Bohorquez',
        descripcion: 'Apasionado por la pedadogía, el cine y de como la palabra Lorem se convierte en la retahíla de letras en Latín (?) en el VSCode',
        codigo: '3',
        image: 'JoseBohorquez.jpg',
        rol: 'Desarrollador BackEnd'
        }"
        ></team-card>

  </div>
</template>

<script>
import TeamCard from './components/TeamCard.vue'

export default {
  name: 'App',
  components: {
  TeamCard
  }
}
</script>

<style lang="stylus" scoped>
  
</style>

