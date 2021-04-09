<template>
  <div>
    <div v-for="(personaje, index) in personajes" :key="index" class="personaje">
      <img :src="personaje.image" />
      <h3>{{ personaje.name }}</h3>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  data: function() {
    return {
      personajes: [
        {
          name: 'Rick Sanchez',
          image: 'https://rickandmortyapi.com/api/character/avatar/1.jpeg'
        },
        {
          name: 'Morty Smith',
          image: 'https://rickandmortyapi.com/api/character/avatar/2.jpeg'
        },
        {
          name: 'Summer Smith',
          image: 'https://rickandmortyapi.com/api/character/avatar/3.jpeg'
        },
          {
          name: 'Beth Smith',
          image: 'https://rickandmortyapi.com/api/character/avatar/4.jpeg'
        },
          {
          name: 'Jerry Smith',
          image: 'https://rickandmortyapi.com/api/character/avatar/5.jpeg'
        }
           
      ]
    }
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.personaje {
  display: flex;
  margin: 15px;
}

.personaje h3 {
  color: #fff;
}

.personaje img {
  width: 100px;
  border-radius: 50%;
}
</style>
