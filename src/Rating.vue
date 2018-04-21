<template>
  <div>
    <ul>
      <li v-for="star in maxStars" :key="star" :class="{ 'is-active': star < stars }" class="star"></li>
    </ul>
  </div>
</template>

<script>
export default {
  data () {
    return {
      stars: 3,
      maxStars: 5
    }
  }
}
</script>
