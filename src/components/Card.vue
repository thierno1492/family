<template>
<div class="container-fluid row row-cols-2 row-cols-lg-5 g-2 g-lg-3">
<div v-for="person in persons"  class="card">
  
    <img alt="Vue logo" src="../assets/item.jpg">
  
  <div class="container" >
    <h4><b>Thierno sadialiou diallo</b></h4> 
    <Show />
    <p>Fils de:Ousmane & Kadiatou toure</p>
    <a href="#">622191010</a>
   <p>Adress:Conakry</p>
   <a href="#">lien parental</a>
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

export default{

   components: {
   
  },
  
    data() {
        return { 
           persons:[{
            "id":1,
            "name":"rojo",
            "age":"25",
            "adress":"conakry",
            "contact":"623246415",
            "work":"house",
            "img": "/src/assets/WIN_20220202_14_58_28_Pro.jpg"

        },
        {
            "id":2,
            "name":"verde",
            "age":"25",
            "adress":"conakry",
            "contact":"623246415",
            "work":"house",
            "img": "/src/assets/item.jpg"
        },
        {
            "id":3,
            "name":"rojo",
            "age":"25",
            "adress":"conakry",
            "contact":"623246415",
            "work":"house",
            "img": "/src/assets/item.jpg"
        },
        {
            "id":4,
            "name":"rojo",
            "age":"25",
            "adress":"conakry",
            "contact":"623246415",
            "work":"house"
        },
        {
            "id":5,
            "name":"rojo",
            "age":"25",
            "adress":"conakry",
            "contact":"623246415",
            "work":"house"
        },
        {   "id":6,
            "name":"rojo",
            "age":"25",
            "adress":"conakry",
            "contact":"623246415",
            "work":"house"
        },
        {   "id":7,
            "name":"rojo",
            "age":"25",
            "adress":"conakry",
            "contact":"623246415",
            "work":"house"
        }
    ]
        }
    },


/* 
    mounted() {
        fetch(' http://localhost:3000/persons')
        .then(res => res.json())
        .then(data =>this.person = data)
          console.log(person)
        .catch(err => console.log(err.message))
  
    }, */
     
     
}


</script>