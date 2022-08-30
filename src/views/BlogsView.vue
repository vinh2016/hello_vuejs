<template>
  <div class="blogs">
    <h1>This is a blogs page</h1>
		<br/>
		<ul>
			<li v-for="value in blogObj">
				{{ value }}
			</li>
		</ul>
  </div>
</template>

<script>
export default {
  name: "Blogs",
  data() {
    return {
      blogObj: {
        title: 'How to do crate an application in Vue',
        author: 'Vinh',
        publishedAt: '2022-08-30'
      }
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
  .blogs {
    min-height: 100vh;
    //display: flex;
    align-items: center;
  }
}
</style>
