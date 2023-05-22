<template>
  <div :class="{ active: isActive }" @click="isActive = !isActive"> 
      <span class="material-symbols-outlined" >
        radio_button_checked
      </span>
  </div>
</template>

<script>
export default {
data(){
    return{
      isActive :false
    }
  },
  watch:{
    isActive(){
        if(this.isActive == true){
          document.body.style.background = "black"
        }
        if(this.isActive == false){
          document.body.style.background = "#f2f2f2"
        }
    },
    
  }
}
</script>

<style>
    span.material-symbols-outlined{
      display: flex;
      direction: rtl;
      margin-right: 50px ;
      margin-top: 30px;
      font-size: 50px;
      cursor: pointer;
      color: #76dd78;

    }
    
    
</style>