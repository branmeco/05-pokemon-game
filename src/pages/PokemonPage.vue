<template>
  <h1>¿Quien es este pokemon?</h1>
  <!--TODO: img-->
  <pokemonPicture :pokemonId="64" :showPokemon="true" />

  <!--TODO: options-->
  <pokemonOptions />
</template>

<script>
import PokemonPicture from "@/components/PokemonPicture.vue";
import PokemonOptions from "@/components/PokemonOptions.vue";

import getPokemonOptions from '../helpers/getPokemonOptions'

// console.log(getPokemonOptions())

export default {
  components: {
    PokemonPicture,
    PokemonOptions,
  },
};
</script>