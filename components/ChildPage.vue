<template>
  <div>
    <!-- don't use mountain.title, just title, since that is the name of the prop that this component knows about -->
    <div class="card" style="width: 18rem;">
      <!-- <img class="card-img-top" src="..." alt="Card image cap"> -->
      <div class="card-body">
        <h5 class="card-title">{{ title }}</h5>
        {{ continent }}<br/>
        {{ height }}
        <ul>
          <li v-for="(country, id) in countries" :key="id ">{{ country }}</li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
// Props declaration and validation
    data() {
      return {
<<<<<<< HEAD

=======
        
>>>>>>> 1bd8ee1ba381a8cf5fac6fe2c0698f50632129b8
      }
    },
    // These props were in the data block above, but should be their own section like this:
    props: {
          title: {
            type: String,
            // required: true,
            default: 'Mountain Title'
          },
          continent: {
            type: String,
            // required: true,
            default: 'Mountain Continent'
          },
          height: {
            type: String,
            // required: true,
            default: 'Mountain Height'
          },
          countries: {
            type: Array,
            // required: true,
            default: 'Mountain Countries'
          }
    }
<<<<<<< HEAD
  }
=======
  }  
>>>>>>> 1bd8ee1ba381a8cf5fac6fe2c0698f50632129b8
</script>
