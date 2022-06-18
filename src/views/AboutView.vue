<template>
  <div class="about">
   <Items />
   <Information />
  </div>
</template>
<script>
import Items from '@/components/Items.vue'
import Information from '@/components/Information.vue'

export default {
  name: 'HomeView',
  components: {
    Items,
    Information
  
  }
}
</script>