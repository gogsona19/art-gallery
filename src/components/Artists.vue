<template>
    <div class="artists">
        <div class="top_info_box">
            <div class="left">
                <span>
                    Artists
                </span>
            </div>
            <div class="right">
                
            </div>
        </div><!--end top info-->
        <div class="artists_wrap">
            <div class="artists_box" >
                <p class="arts_pharagraph" v-for="data in artists.slice(0, 17)" :key="data.id">
                        {{data}}
                </p>    
            </div>
            <div class="artists_box">
                <p class="arts_pharagraph" v-for="data in artists.slice(17, 34)" :key="data.id">
                        {{data}}
                </p>  
            </div>
            <div class="artists_box">
                <p class="arts_pharagraph" v-for="data in artists.slice(34, 51)" :key="data.id">
                        {{data}}
                </p> 
            </div>
            <div class="artists_box">
                <div class="arts_image_box">
                    <img src="../assets/user.png" alt="artists">
                </div>
            </div>

        </div>
        
    </div>
</template>
<script>
export default {
        data : ()=> ({
            artists : ['Franz Ackermann', 'Etel Adnan', 'Darren Almond','Ellen Altfest ','Michael Armitage','Miroslaw Balka','Georg Baselitz',
            'Larry Bell','Jake & Dinos Chapman','Chuck Close','Gregory Crewdson','Tracey Emin','Katharina Fritsch','Theaster Gates','Gilbert & George','Antony Gormley',
            'Andreas Gursky','David Hammons','Mona Hatoum','He Xiangyu ','Damien Hirst','Robert Irwin ','Runa Islam ','Sergej Jensen ','Anselm Kiefer','Rachel Kneebone','Imi Knoebel','Elad Lassry','Liza Lou','Jac Leirner','Liu Wei','Christian Marclay','Josiah McElheny','Julie Mehretu',
            'Beatriz Milhazes','Harland Miller','Sarah Morris ','Gabriel Orozco','Damián Ortega','Virginia Overton','Eddie Peake','Magnus Plessen','Jessica Rankin','Christian Rosa','Doris Salcedo','Raqib Shaw','Haim Steinbach','Sam Taylor-Johnson','Fred Tomaselli','Jeff Wall','Cerith Wyn Evans'],
        }),
    mounted(){
           
    },
    methods : {

    }
}
</script>
<style scoped>
    .artists{
        width: 100%;
        min-height: 600px;
        margin-top: 50px;
        float: left;
         border-top: 1px solid #D8D8D8;
    }
        .top_info_box{
        display: grid;
        grid-template-columns: 50% 50%;
        font-size: 24px;
        padding: 10px 0;
    }
    .top_info_box .left{
        text-align: left;
    }
    .top_info_box .right{
        text-align: right;
    }
    .artists_wrap{
        display: grid;
        grid-template-columns: 25% 25% 25% 25%;
        width: 100%;
        min-height: 600px;
    }
    .artists_box{
        width: 100%;
        min-height: 700px;
    }
    .arts_pharagraph{
        text-align: left;
    }
    .arts_image_box{
        width: 220px;
        height: 220px;
    }
    .arts_image_box img{
        width: 100%;
        height: 100%;
    }
       @media (max-width: 768px) {
       .arts_image_box{
           display: none;
       }
       .artists_wrap{
           display: block !important;
       }
   }
</style>