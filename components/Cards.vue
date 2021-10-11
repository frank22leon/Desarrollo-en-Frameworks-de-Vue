<template>
  <div>
    <b-row>
      <b-col cols-md="4" v-for="(personaje, index) in personajes" :key="index">
        <b-card
          :title="personaje.nombre"
          :img-src="personaje.imagen"
          img-alt="Image"
          img-top
          tag="article"
          style="max-width: 20rem;"
          class="mb-5"
        >
        </b-card>
      </b-col>
    </b-row>
  </div>
</template>

<script>
export default {
  data: () => ({
    personajes: [
      {
        id: 1,
        nombre: "Morty",
        imagen: "https://rickandmortyapi.com/api/character/avatar/2.jpeg",
      },
      {
        id: 2,
        nombre: "Rick",
        imagen: "https://rickandmortyapi.com/api/character/avatar/1.jpeg",
      },
      {
        id: 3,
        nombre: "Summer",
        imagen: "https://rickandmortyapi.com/api/character/avatar/3.jpeg",
      },
      {
        id: 4,
        nombre: "Beth",
        imagen: "https://rickandmortyapi.com/api/character/avatar/4.jpeg",
      },
      {
        id: 5,
        nombre: "Jerry",
        imagen: "https://rickandmortyapi.com/api/character/avatar/5.jpeg",
      },
    ],
  }),
};
</script>

<style></style>
