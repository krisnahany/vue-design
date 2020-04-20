<template>
    <div class="col-3 reset">
        <div class="title">
            <button class="left"><i class="fa fa-angle-down"></i></button>
            <p class="left">Participant</p>
            <button class="right"><i class="fa fa-times"></i></button>
            <div class="clearfix"></div>
        </div>
        <div class="participant">
            <ul v-for="(obj, key) in participant_list" :key="key">
                <li>
                    <img class="left" :src="obj.img" :alt="obj.alt">
                    <p class="left">{{ obj.nama }}</p>
                    <button class="right"><i class="fa fa-microphone-slash red" style=""></i></button>
                    <button class="right"><i class="fa fa-video-camera blue" style=""></i></button>
                    <div class="clearfix"></div>
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    props:['participant_list'],
    name: 'Participant'
}
</script>

<style lang="css">
    .col-3.reset{
        padding: 0;
        background-color: white;
    }

    .col-3 .title {
        background-color: #F5F5F6;
    }

    .col-3 .title .left, .right{
        margin: 5px 10px;
    }

    .col-3 .participant {
        margin: 5px 15px;
    }

    .col-3 .participant ul {
        text-align: left;
        margin: 0;
        padding: 0;
    }

    .col-3 .participant ul li {
        list-style: none;
    }
    
    .col-3 .participant ul li p.left {
        margin: 0;
        padding: 0 5px 5px 5px;
        margin-left: 3px;
        font-size: 14px;
    }

    .col-3 .participant ul li img.left {
        border-radius: 50%;
        width: 20px;
        height: 20px;
        margin: 2px 0;
    }

    .col-3 .participant ul li button {
        margin: 0;
    }

    .col-3 .participant ul li button .red {
        color: #F74B41;
    }

    .col-3 .participant ul li button .blue {
        color: #00BCEB;
    }
</style>