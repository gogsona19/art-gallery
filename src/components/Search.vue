<template>
        <div class="searchs" v-if="showSearch">
            <input type="text" class="form-control" placeholder="Search..." aria-label="Search..." aria-describedby="basic-addon1">
        </div>
    <div class="search_box">
        <button class="btn btn-link btn-lg" @click="showSearch =! showSearch" type="button" >
               <i class="bi bi-search"></i>
        </button>
    </div>
</template>

<style scoped>
.search_box{
    float: right;
}
.searchs {
    width: 80%;
    margin-top: 5px;
    float: left;
}
</style>
<script>
export default {
    data : ()=> ({
    showSearch : false,
  }),
    mounted(){
           
    },
    methods : {

    }

}
</script>