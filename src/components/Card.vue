<template>
<div class="container-fluid row row-cols-2">
<div v-for="person in persons"  class="card">
  
    <img alt="Vue logo" src="../assets/WIN_20220202_14_58_28_Pro.jpg">
  
  <div class="container" >
    <h4><b>{{person.name}}</b></h4> 
    <Show />
    <p>Fils de:Ousmane & Kadiatou toure</p>
    <a href="#">{{person.conctact}}</a>
   <p>Adress:{{person.address}}</p>
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
.container-fluid[data-v-54cdc180] {
    display: flex;
}
.container {
  padding: 2px 16px;
  }
  .container-fluid{
    display: flex;
  }
  .row {
    display: -ms-flexbox;
    display: flex;
    -ms-flex-wrap: wrap;
    flex-wrap: wrap;
    margin-right: 0;
    margin-left: 0;

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
            "name":"saliou",
            "age":"25",
            "adress":"conakry",
            "contact":"623246415",
            "work":"house",
            "img": "/src/assets/WIN_20220202_14_58_28_Pro.jpg"

        },
        {
            "id":2,
            "name":"mamadou",
            "age":"25",
            "adress":"conakry",
            "contact":"623246415",
            "work":"house",
            "img": "/src/assets/item.jpg"
        },
        {
            "id":3,
            "name":"samba",
            "age":"25",
            "adress":"conakry",
            "contact":"623246415",
            "work":"house",
            "img": "/src/assets/item.jpg"
        },
        {
            "id":4,
            "name":"bhoye",
            "age":"25",
            "adress":"conakry",
            "contact":"623246415",
            "work":"house"
        },
        {
            "id":5,
            "name":"mamadian",
            "age":"25",
            "adress":"conakry",
            "contact":"623246415",
            "work":"house"
        },
        {   "id":6,
            "name":"cellou",
            "age":"25",
            "adress":"conakry",
            "contact":"623246415",
            "work":"house"
        },
        {   "id":7,
            "name":"kadiatou",
            "age":"25",
            "adress":"conakry",
            "contact":"623246415",
            "work":"house"
        ,
        },
          {
            "id":8,
            "name":"mamadian",
            "age":"25",
            "adress":"conakry",
            "contact":"623246415",
            "work":"house"
        },
        {   "id":9,
            "name":"cellou",
            "age":"25",
            "adress":"conakry",
            "contact":"623246415",
            "work":"house"
        },
        {   "id":10,
            "name":"kadiatou",
            "age":"25",
            "adress":"conakry",
            "contact":"623246415",
            "work":"house"
        ,
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