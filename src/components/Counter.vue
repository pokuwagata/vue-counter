<template>
  <div>
    <p>{{count}}</p>
    <p>{{double}}</p>
    <p v-if="count === 5">5</p>
    <button @click="increment">+</button>
    <button @click="decrement">-</button>
  </div>
</template>

<script>
export default {
  name: 'Counter',
  data: function() {
    return {
      count: 0
    }
  },
  methods: {
    increment: function() {
      this.count++
    },
    decrement: function() {
      this.count--
    }
  },
  computed: {
    double: function() {
      return this.count * 2
    }
  }
}
</script>

