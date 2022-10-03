<template>
  <div>
<h1>Mountains API child component</h1>
<ul>
  <li>{{ mountains.title }}</li>
  <li>{{ mountains.continent }}</li>
  <li>{{ mountains.height }}</li>
  <li>{{ mountains.countries }}</li>
</ul>
</div>
</template>

<script>
  export default {
// Props declaration and validation
    data() {
      return {
        props: {
          title: {
            type: String,
            required: true
          },
          continent: {
            type: String,
            required: true
          },
          height: {
            type: String,
            required: true
          },
          countries: {
            type: String,
            required: true
          }
        }
      }
    }
  }
</script>
