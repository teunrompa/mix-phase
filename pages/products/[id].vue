<template>
  <div>
    <p>Product details for {{ id }}</p>
    <p>
      Lorem, ipsum dolor sit amet consectetur adipisicing elit. Beatae ad
      accusantium, nesciunt cupiditate cum illo nisi suscipit voluptatum
      architecto nihil asperiores magni adipisci ratione inventore animi!
      Impedit magnam alias numquam?
    </p>
  </div>
</template>

<script setup>
const { id } = useRoute().params;
</script>

<style  scoped>

</style>
