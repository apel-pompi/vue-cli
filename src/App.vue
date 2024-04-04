<template>
    
    <div>
      <ListHelperVue>
        
      </ListHelperVue>
      
    </div>

</template>

<script>
import ListHelperVue from './components/ListHelper.vue'
export default {

  data(){
    return {
      list: ['html','css','php','java'],
      loader:''
    }
  },
  components:{
    ListHelperVue
  },
  created(){
    setTimeout(()=>{
      this.loader = 'other'
    },3000)
  }
  
}
</script>

