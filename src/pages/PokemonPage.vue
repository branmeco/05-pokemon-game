<template>
  <h1>¿Quien es este pokemon?</h1>
  <!--TODO: img-->
  <pokemonPicture />

  <!--TODO: options-->
  <pokemonOptions />
</template>

<script>
import PokemonPicture from "@/components/PokemonPicture.vue";
import PokemonOptions from "@/components/PokemonOptions.vue";

export default {
  components: {
    PokemonPicture,
    PokemonOptions,
  },
};
</script>