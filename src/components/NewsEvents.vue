<template>
    <div class="news_events">
        <div class="top_info_box">
            <div class="left">
                <span>
                    News & Events
                </span>
            </div>
            <div class="right">
                <span>
                    View all<i class="bi bi-arrow-right-short"></i>
                </span>
            </div>
        </div><!--end top info-->
        <div class="news_events_post_box">
            <div class="post_box">
                <div class="image_box">
                    <img src="../assets/01.png" alt="art gallery">
                </div>
                <div class="post_text_box">
                    <p class="card-text">
                        Exhibition: He Xiangyu monograph released by Distanz
From March 2016<br>
He Xiangyu and Liu Wei are among 74 international artists from 33 countries chosen to feature in the Yinchuan Biennale 2016
                    </p>
                </div>
            </div>
            <div class="post_box">
                <div class="image_box">
                    <img src="../assets/02.png" alt="art gallery">
                </div>
                <div class="post_text_box">
                    <p class="card-text">
                        Exhibition: He Xiangyu monograph released by Distanz
From March 2016<br>
He Xiangyu and Liu Wei are among 74 international artists from 33 countries chosen to feature in the Yinchuan Biennale 2016
                    </p>
                </div>
            </div>
            <div class="post_box">
                <div class="image_box">
                    <img src="../assets/03.png" alt="art gallery">
                </div>
                <div class="post_text_box">
                    <p class="card-text">
Preview: White Cube Mason’s Yard
19 January 2017, 6 to 8pm<br>
Join us at Mason's Yard, London for the preview of the new Park Seo-Bo exhibition curated by Katharine Kostyál. Curated by Katharine Kostyál
                    </p>
                </div>
            </div>
            
            
            
            <!--
            <div class="post_box" v-for="data in newsData" :key="data.id">
                <div class="image_box">
                    <img :src="data.img" alt="art gallery">
                </div>
                <div class="post_text_box"><p>{{data.description}}</p>
                </div>
            </div>-->

        </div>
    </div>
</template>
<script>
export default {
    data : ()=> ({
        newsData  :[
            {
                id : 1,
                img: 'http://localhost:8080/img/01.png',
                description : 'Exhibition: He Xiangyu monograph released by Distanz From March 2016 <br He Xiangyu and Liu Wei are among 74 international artists from 33 countries chosen to feature in the Yinchuan Biennale 2016',

            },
            {
                id : 2,
                img: '../assets/02.png',
                description : 'Exhibition: He Xiangyu monograph released by Dist anzFrom March 2016<br>He Xiangyu and Liu Wei are among 74 international artists from 33 countries chosen to feature in the Yinchuan Biennale 2016',

            },
            {
                id : 3,
                img: '../assets/03.png',
                description : 'Preview: White Cube Mason’s Yard 19 January 2017, 6 to 8pm<br>Join us at Mason s Yard, London for the preview of the new Park Seo-Bo exhibition curated by Katharine Kostyál. Curated by Katharine Kostyál',

            }
        ]
    }),
    mounted(){
           
    },
    methods : {

    }
}
</script>
<style scoped>
    .news_events{
        width: 100%;
        height: 600px;
       /* background-color: brown;*/
        float: left;
        margin-top: 50px;
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
    .news_events_post_box{
        display: grid;
        grid-template-columns: 330px 330px 300px;
    }
    .image_box{
        width: 300px;
        height: 300px;
    }
    .image_box img{
        width: 100%;
    }
    .post_text_box {
    width: 94%;
    height: 215px;
    text-align: left;
    margin-top: 15px;
    overflow: hidden;
}
   .post_text_box p {
       color: #262626;
       font-size: 20px;
      
   }
   @media (max-width: 768px) {
       .news_events_post_box{
           display: block;
       }
       .news_events{
           height: 100%;
           margin-top:30px;
       }
       .image_box{
           width: 100%;
           height: 100%;
       }
   }
</style>