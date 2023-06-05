<template>
  <h1>¿Quien es este pokemon?</h1>
  <!--TODO: img-->
  <pokemonPicture :pokemonId="64" :showPokemon="true" />

  <!--TODO: options-->
  <pokemonOptions :pokemons="pokemonArr"/>
</template>

<script>
import PokemonPicture from "@/components/PokemonPicture.vue";
import PokemonOptions from "@/components/PokemonOptions.vue";

import getPokemonOptions from '../helpers/getPokemonOptions'

export default {
  components: {
    PokemonPicture,
    PokemonOptions,
  },
  data() {
    return {
      pokemonArr: []
    }
  },
  methods: {
    async mixPokemonArr(){
      this.pokemonArr = await getPokemonOptions()
    }
  },
  mounted() {
    this.mixPokemonArr()
  }
};
</script>