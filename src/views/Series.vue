<template>
<v-container>
    <v-row >
        <v-col cols="12" sm="4" md="4" lg="4" v-for="personaje in personajes" :key="personaje.nombre"><v-card
        class="mx-auto"
        max-width="400"
        >
        <v-img
        height="200px"
        :src="personaje.imagen"
        >
        </v-img>

        <v-card-subtitle class="pb-0" >
        {{personaje.nombre}}
        </v-card-subtitle>



    </v-card>
  </v-col>
</v-row>
</v-container>
</template>

<script>
export default {
    name: 'component-series',
    // props: {},
    data () {
        return{
            personajes:[
            {
            id: 1,
            nombre:'Morty',
            imagen:  'https://rickandmortyapi.com/api/character/avatar/2.jpeg'
            },
            {
            id: 2,
            nombre:'Rick',
            imagen: 'https://rickandmortyapi.com/api/character/avatar/1.jpeg'

            },
              {
            id: 3,
            nombre:'Summer',
            imagen: 'https://rickandmortyapi.com/api/character/avatar/3.jpeg'

            },
              {
            id: 4,
            nombre:'Beth',
            imagen: 'https://rickandmortyapi.com/api/character/avatar/4.jpeg'

            },
              {
            id: 5,
            nombre:'Jerry',
            imagen: 'https://rickandmortyapi.com/api/character/avatar/5.jpeg'

            }
        ]
        }
    },
    // computed: {},
    methods: {
        // -- Metodos
    },
    // components: {},
}
</script>

<style scoped>

</style>