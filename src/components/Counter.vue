<template>
  <div>
    <p>{{count}}</p>
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
  }
}
</script>

