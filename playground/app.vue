<script setup lang="ts">
import { parse } from 'graphql'

const query = parse(`
  query QueryHello($name: String) {
    hello(name: $name)
  }
`)
</script>

<template>
  <div>
    {{ query }}
  </div>
</template>
