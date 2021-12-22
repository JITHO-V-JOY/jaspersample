<template>
    <div>
        <iframe class="example" v-bind:src="url+'?j_username='+username+'&j_password='+password" width="1000" height="1000" ></iframe>

    </div>
</template>

<script>
export default {
 name:"ReportComponent",
 props:{
     username: String,
     password: String,
     url:String
 }
 
}
</script>

<style scoped>
    iframe{
        border: none;
        scroll-margin: none;
        
    }
    .example::-webkit-scrollbar {
  display: none;
}
</style>