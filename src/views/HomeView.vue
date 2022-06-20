<template>
  <div class="home">

  <Card />
    <Items />
  </div>
</template>

<script>
// @ is an alias to /src

import Card from '@/components/Card.vue'

export default {
  name: 'HomeView',
  components: {
   
    Card
  },
    data() {
        return { 
            persons: []
        }
    },

 /*    mounted() {
        fetch(' http://localhost:3000/persons')
        .then(res => res.json())
        .then(data =>this.persons = data)
        .catch(err => console.log(err.message))
    } */
}
</script>
