<template>
  <div>
      <ul class="list">
          <li v-for="beer in favouriteBeers" :favouriteBeer="beer" :key="beer.id">{{beer.name}}</li>
      </ul>
  </div>
</template>

<script>
export default {
    name: "list-favourite-beers",
    props: ['favouriteBeers']
}
</script>

<style scoped>
    .list {
        list-style: none;
    }
</style>