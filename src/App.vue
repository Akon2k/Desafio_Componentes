<template>
  <div>
    <div v-for="(personaje, i) in personajes" :key="i" class="personaje">
      <img :src="personaje.image" />
      <div style="padding-top: 60px">
        <h2>{{ personaje.name }}</h2>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  data: function () {
    return {
      personajes: [
        {
          name: "Rick Sanchez",
          image: "https://rickandmortyapi.com/api/character/avatar/1.jpeg",
        },
        {
          name: "Morty Smith",
          image: "https://rickandmortyapi.com/api/character/avatar/2.jpeg",
        },
        {
          name: "Summer Smith",
          image: "https://rickandmortyapi.com/api/character/avatar/3.jpeg",
        },
        {
          name: "Beth Smith",
          image: "https://rickandmortyapi.com/api/character/avatar/4.jpeg",
        },
        {
          name: "Jerry Smith",
          image: "https://rickandmortyapi.com/api/character/avatar/5.jpeg",
        },
        {
          name: "Abadango Cluster Princess",
          image: "https://rickandmortyapi.com/api/character/avatar/6.jpeg",
        },
      ],
    };
  },
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

.personaje img {
  width: 125px;
  border-radius: 50%;
}

.personaje h2 {
  color: #ff0000;
}
</style>
