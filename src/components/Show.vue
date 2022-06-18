<template>
<div>

</div>
</template>
<script>
export default{
  props:['img'],
    data() {
        return { 
            person: null,
            img
        }
    },

  mounted() {
        fetch(`http://localhost:3000/persons/${this.id}/img`)
       
        .then(data =>this.img = data)
          console.log(person)
        .catch(err => console.log(err.img))
  
    }
}


</script>