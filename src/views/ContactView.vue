<template>
  <div class="contact">
    <h1>This is a contact page</h1>
    <button @click="count++">Say hi</button>
    <p>Count is: {{ count }}</p>
  </div>
</template>

<script>
export default {
  name: "Contact",
  data() {
    return {
      count: 0
    };
  },
  methods: {
    searchFunc: function () {},
  },
  props: {
    content: {},
  },
};
</script>

<style>
@media (min-width: 1024px) {
  .contact {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}
</style>
