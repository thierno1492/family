<template>
<div class="container-fluid row row-cols-2 row-cols-lg-5 g-2 g-lg-3">
<div   v-for="persons in person" :key="person.id" class="card">
  
    <img alt="Vue logo" src="../assets/item.jpg">
  
  <div class="container" >
    <h4><b>{{persons.name}}</b></h4> 
    <p>Architect & Engineer</p> 
    <p>{{persons.age}}</p>
    <p>Fils de:Ousmane & Kadiatou toure</p>
    <a href="#">{{persons.contact}}</a>
   <p>Adress:Conakry</p>
  </div>
</div>
</div>
</template>
<style scoped>
.card {
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
  transition: 0.3s;
  width: 40%;
}

.card:hover {
  box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
}

.container {
  padding: 2px 16px;
  }
  .container-fluid{
    display: flex;
  }
</style>

<script>
import Show from '@/components/Show.vue'
export default{

   components: {
   
    Show
  },
  
    data() {
        return { 
            person: null,
            img: ""
        }
    },

    mounted() {
        fetch(' http://localhost:3000/persons')
        .then(res => res.json())
        .then(data =>this.person = data)
          console.log(person)
        .catch(err => console.log(err.message))
  
    },
     
     
}


</script>