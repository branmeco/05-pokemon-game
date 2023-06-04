<template>
  <h1>¿Quien es este pokemon?</h1>
  <!--TODO: img-->
  <pokemonPicture />

  <!--TODO: options-->
  <pokemonOption />
</template>

<script>
import PokemonPicture from "@/components/PokemonPicture.vue";
import PokemonOption from "@/components/PoekemonOption.vue";

export default {
  components: {
    PokemonPicture,
    PokemonOption,
  },
};
</script>