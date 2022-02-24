<template>
    <div>
     
            <button class="btn btn-link btn-lg" type="button" data-bs-toggle="collapse" data-bs-target="#collapseExample" aria-expanded="false" aria-controls="collapseExample">
                <i class="bi bi-list"></i>
            </button>
    
        <div class="collapse" id="collapseExample">
        <div class="card card-body">
                <router-link to="/">Home</router-link> 
                <router-link to="/Art">Art & Artists</router-link>
                <router-link to="/Exhibitions">Exhibitions</router-link> 
                <router-link to="/News">News</router-link>
                <router-link to="/About">About</router-link> 
                <router-link to="/Private">Private area</router-link>
        </div>
        </div>
    </div>
</template>
<style scoped>
i.bi.bi-list {
    color: black;
    font-weight: bold;
    font-size: 28px;
}
   @media (max-width: 768px) {
       #nav a{
           font-size: 30px;
       }
   }


</style>