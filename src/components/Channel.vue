<template>
    <div class="channel">
        <div class="top_info_box">
            <div class="left">
                <span>
                    Channel
                </span>
            </div>
            <div class="right">
                <span>
                    View all<i class="bi bi-arrow-right-short"></i>
                </span>
            </div>
        </div><!--end top info-->
        <div class="embed-responsive embed-responsive-16by9">
            <iframe class="embed-responsive-item" src="https://www.youtube.com/embed/zpOULjyy-n8?rel=0" allowfullscreen></iframe>
        </div>
        <div class="bottom_info_box">
            <div>
                <p>
                    Anselm Kiefer in conversation with Tim Marlow in the Auditorium
                </p>
            </div>
            <div>
                <p>
                    In this film Anselm Kiefer discusses his work and his exhibition ‘Walhalla’ at White Cube Bermondsey with Tim Marlow.
                </p>
            </div>
        </div>
    </div>
</template>
<style scoped>
.channel{
    width: 100%;
    min-height: 600px;
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
    .bottom_info_box{
        display: grid;
        grid-template-columns: 48% 50%;
    }
    .bottom_info_box div p{
        font-size: 20px;
        text-align: left;
        padding: 10px 0;
    }
       @media (max-width: 768px) {
           .bottom_info_box{
               display: block;
           }
            }
</style>