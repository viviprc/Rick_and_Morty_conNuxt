<template>
  <v-app>
    <v-main class="pt-0">
      <v-container>
        <v-row>
          <v-col md="4" v-for="(personaje, i) in personajes" :key="i">
            <v-card class="mx-auto" max-width="300">
              <v-img
                class="white--text align-end"
                height="200px"
                :src="personaje.imagen"
              >
              </v-img>

              <v-card-title class="pb-0"> {{ personaje.nombre }} </v-card-title>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
export default {
  data() {
    return {
      personajes: [
        {
          id: 1,
          nombre: 'Morty',
          imagen: 'https://rickandmortyapi.com/api/character/avatar/2.jpeg',
        },
        {
          id: 2,
          nombre: 'Rick',
          imagen: 'https://rickandmortyapi.com/api/character/avatar/1.jpeg',
        },
        {
          id: 3,
          nombre: 'Summer',
          imagen: 'https://rickandmortyapi.com/api/character/avatar/3.jpeg',
        },
        {
          id: 4,
          nombre: 'Beth',
          imagen: 'https://rickandmortyapi.com/api/character/avatar/4.jpeg',
        },
        {
          id: 5,
          nombre: 'Jerry',
          imagen: 'https://rickandmortyapi.com/api/character/avatar/5.jpeg',
        },
      ],
    }
  },
}
</script>
