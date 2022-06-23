<template>
  <div class="container-fluid item">
    <div class="card"  v-for="person in persons">
<div class="aw">  <img :src="person.img" :alt="logo"></div>
  <div class="card-body">
    <h5 class="card-title">{{ person.name }}</h5>
     <p class="card-text">Age:{{ person.age }}</p>
     <a href="#">Tel:{{ person.contact}}</a>
    
  </div>
  <ul class="list-group list-group-flush">
 
    
    <li class="list-group-item">Filiation:{{person.filiation}}</li>
    <li class="list-group-item">Address:{{ person.adress }}</li>
  </ul>
  <div class="card-body">
    <p  class="card-link">Fbk: {{ person.social}}</p>
    <a href="#" class="card-link">lien familial</a>
     <p>Profession:{{ person.work }}</p>
  </div>
</div>
  </div>
</template>
<style scoped>
.card {
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2);
  transition: 0.3s;
  width: 40%;
}
.item{
  display: grid;
  grid-template-columns: repeat(4, 1fr);

  
}
h5{
  color: black;
}
li{
  font-size:9px;
}
.aw{
  
  height:60vh;
}
.aw img{
  width:100%;
  height:59vh;
}
.card{
    border: 5px inset #1C6EA4;
    width:100%;
}
.card:hover {
  box-shadow: 0 8px 16px 0 rgba(0, 0, 0, 0.2);
}

.container-fluid {
  padding: 0;

  box-sizing: border-box;
  width: 100%;
  
}

.row {
  display: -ms-flexbox;
  display: flex;
  -ms-flex-wrap: wrap;
  flex-wrap: wrap;
  margin-right: 0;
  margin-left: 0;
}

@media screen and (max-width: 1107px) {
 .item{
  display: grid;
  grid-template-columns: repeat(3, 1fr);

  
}
  }

  @media screen and (max-width: 894px) {
 .item{
  display: grid;
  grid-template-columns: repeat(3, 1fr);

  
}

  @media screen and (max-width: 689px) {
 .item{
  display: grid;
  grid-template-columns: repeat(2, 1fr);

  }
  .aw img[data-v-54cdc180] {
  width: 100%;
  height: 36vh;
}
.aw[data-v-54cdc180] {
  height: 35vh;
}
}
  }
</style>

<script>
export default {
  components: {},

  data() {
    return {
      persons: [
        {
          id: 1,
          name: "Mdou saliou diallo",
          age: "30",
          adress: "Dakar senegal",
          contact: "+221778593204",
          work: "Gestionnaire",
          img: "https://curious-fox-r9fg36-dev-ed--c.documentforce.com/sfc/dist/version/renditionDownload?rendition=ORIGINAL_Jpg&versionId=0687Q000000VqCf&operationContext=DELIVERY&contentId=05T7Q000009auql&page=0&d=/a/7Q000000GoXX/g9lDlnuOzMcSQ3yjaZRgPG0QjEHlsG1A44rltkAYN.Y&oid=00D7Q000004syll&dpt=null&viewId=",
          filiation: "Mousou wondjira",
          social: " Xaliou Diallo",
        },
        {
          id: 2,
          name: "Th mamadou Diallo",
          age: "22",
          adress: "Kindia guinee",
          contact: "+221778593204 ",
          work: "Gestionnaire ",
          filiation: "Ousmane & binta diallo",
          social: "Mamadou Gaoual Diallo",
          img: "https://curious-fox-r9fg36-dev-ed--c.documentforce.com/sfc/dist/version/renditionDownload?rendition=ORIGINAL_Jpeg&versionId=0687Q000000VqCV&operationContext=DELIVERY&contentId=05T7Q000009auqb&page=0&d=/a/7Q000000GoXb/MGKT1DkAPhHpPCaIIOCO6I8xLkPENYqtzpTDCBnE3B8&oid=00D7Q000004syll&dpt=null&viewId=",
        },
        {
          id: 3,
          name: "Th sadialiou diallo",
          age: "29",
          adress: "Espagne madrid",
          contact: "+34623246515",
          work: "Fullstack developer",
          img: "https://curious-fox-r9fg36-dev-ed--c.documentforce.com/sfc/dist/version/renditionDownload?rendition=ORIGINAL_Jpg&versionId=0687Q000000Vqij&operationContext=DELIVERY&contentId=05T7Q000009axTa&page=0&d=/a/7Q000000GoXq/7hWwiZ0egQppPFmSQQWAtF_xrGhka16rnEST9tIXjSQ&oid=00D7Q000004syll&dpt=null&viewId=",
          filiation: "ousmane & kadiatou toure",
          social: "Thierno Diallo",
        },
        {
          id: 4,
          name: "Ousmane Diallo",
          age: "23",
          adress: "conakry",
          contact: "+13472169289",
          work: "house",
          filiation: "Boubacar & mahawa tounkara",
          social: "Ousmane Diallo",
        img: "https://curious-fox-r9fg36-dev-ed--c.documentforce.com/sfc/dist/version/renditionDownload?rendition=ORIGINAL_Jpg&versionId=0687Q000000VqBE&operationContext=DELIVERY&contentId=05T7Q000009auq2&page=0&d=/a/7Q000000GoXv/IXwwggrRXGC1n_U90rQ12O1cVdzQMU9glDONbRgHV2s&oid=00D7Q000004syll&dpt=null&viewId=",
        },
        {
          id: 5,
          name: "mamadian",
          age: "25",
          adress: "conakry",
          contact: "623246415",
          work: "house",
          filiation: "Mamadou et bella oury",
          filiation: "Mamadou et bella oury",
          social: "https://www.facebook.com/thienomamadoukoumbia.diallo",
            img: "https://curious-fox-r9fg36-dev-ed--c.documentforce.com/sfc/dist/version/renditionDownload?rendition=ORIGINAL_Jpg&versionId=0687Q000000Vqij&operationContext=DELIVERY&contentId=05T7Q000009axTa&page=0&d=/a/7Q000000GoXq/7hWwiZ0egQppPFmSQQWAtF_xrGhka16rnEST9tIXjSQ&oid=00D7Q000004syll&dpt=null&viewId=",
        },
        {
          id: 6,
          name: "cellou",
          age: "25",
          adress: "conakry",
          contact: "623246415",
          work: "house",
          filiation: "Mamadou et bella oury",
          filiation: "Mamadou et bella oury",
          social: "https://www.facebook.com/thienomamadoukoumbia.diallo",
         img: "https://curious-fox-r9fg36-dev-ed--c.documentforce.com/sfc/dist/version/renditionDownload?rendition=ORIGINAL_Jpg&versionId=0687Q000000Vqij&operationContext=DELIVERY&contentId=05T7Q000009axTa&page=0&d=/a/7Q000000GoXq/7hWwiZ0egQppPFmSQQWAtF_xrGhka16rnEST9tIXjSQ&oid=00D7Q000004syll&dpt=null&viewId=",
        },
        {
          id: 7,
          name: "kadiatou",
          age: "25",
          adress: "conakry",
          contact: "623246415",
          work: "house",
          filiation: "Mamadou et bella oury",
          filiation: "Mamadou et bella oury",
          social: "https://www.facebook.com/thienomamadoukoumbia.diallo",
           img: "https://curious-fox-r9fg36-dev-ed--c.documentforce.com/sfc/dist/version/renditionDownload?rendition=ORIGINAL_Jpg&versionId=0687Q000000Vqij&operationContext=DELIVERY&contentId=05T7Q000009axTa&page=0&d=/a/7Q000000GoXq/7hWwiZ0egQppPFmSQQWAtF_xrGhka16rnEST9tIXjSQ&oid=00D7Q000004syll&dpt=null&viewId=",
        },
        {
          id: 8,
          name: "mamadian",
          age: "25",
          adress: "conakry",
          contact: "623246415",
          work: "house",
          filiation: "Mamadou et bella oury",
          filiation: "Mamadou et bella oury",
          social: "https://www.facebook.com/thienomamadoukoumbia.diallo",
       img: "https://curious-fox-r9fg36-dev-ed--c.documentforce.com/sfc/dist/version/renditionDownload?rendition=ORIGINAL_Jpg&versionId=0687Q000000Vqij&operationContext=DELIVERY&contentId=05T7Q000009axTa&page=0&d=/a/7Q000000GoXq/7hWwiZ0egQppPFmSQQWAtF_xrGhka16rnEST9tIXjSQ&oid=00D7Q000004syll&dpt=null&viewId=",
        },
        {
          id: 9,
          name: "cellou",
          age: "25",
          adress: "conakry",
          contact: "623246415",
          work: "house",
          filiation: "Mamadou et bella oury",
          filiation: "Mamadou et bella oury",
          social: "https://www.facebook.com/thienomamadoukoumbia.diallo",
           img: "https://curious-fox-r9fg36-dev-ed--c.documentforce.com/sfc/dist/version/renditionDownload?rendition=ORIGINAL_Jpg&versionId=0687Q000000Vqij&operationContext=DELIVERY&contentId=05T7Q000009axTa&page=0&d=/a/7Q000000GoXq/7hWwiZ0egQppPFmSQQWAtF_xrGhka16rnEST9tIXjSQ&oid=00D7Q000004syll&dpt=null&viewId=",
        },
        {
          id: 10,
          name: "kadiatou",
          age: "25",
          adress: "conakry",
          contact: "623246415",
          work: "house",
          filiation: "Mamadou et bella oury",
          filiation: "Mamadou et bella oury",
          social: "https://www.facebook.com/thienomamadoukoumbia.diallo",
            img: "https://curious-fox-r9fg36-dev-ed--c.documentforce.com/sfc/dist/version/renditionDownload?rendition=ORIGINAL_Jpg&versionId=0687Q000000Vqij&operationContext=DELIVERY&contentId=05T7Q000009axTa&page=0&d=/a/7Q000000GoXq/7hWwiZ0egQppPFmSQQWAtF_xrGhka16rnEST9tIXjSQ&oid=00D7Q000004syll&dpt=null&viewId=",
        },
      ],
    };
  },

  /* 
    mounted() {
        fetch(' http://localhost:3000/persons')
        .then(res => res.json())
        .then(data =>this.person = data)
          console.log(person)
        .catch(err => console.log(err.message))
  
    }, */
};
</script>
