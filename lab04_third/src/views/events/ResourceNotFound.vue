<template>
  <div>
    <h1>Omg!</h1>
    <h3>The "{{ resource }}" that you're looking for is not here.</h3>
    <router-link :to="{ name: 'home' }">Back to the home page</router-link>
  </div>
</template>

<script>
export default {
  props: {
    resource: {
      type: String,
      required: true,
      default: "page",
    },
  },
};
</script>
