<template>
    <div class="">
        <header class="row">
            <div class="logo "><h1>ART GALLERY</h1></div>
                <div class="search ">
                <Top_Menu />
                <Search />
            </div>
        </header>
    </div>
</template>
<script>

import Search from "@/components/Search.vue";
import Top_Menu from "@/components/Top_Menu.vue";
export default {
    components : {
        Search,
        Top_Menu,
    }
}
</script>
<style >
div#collapseExample {
    position: absolute;
    width: 100%;
    left: 0;
     top: 4%;
}
.row{
    display: grid;
    grid-template-columns: 35% 65%;
    
}
.logo h1 {
    text-align: left;
}
button.btn.btn-link.btn-lg {
    line-height: 27px;
    float: right;
}

@media (max-width: 768px) {
.logo h1 {
    font-size: 24px;
}
  
}


</style>