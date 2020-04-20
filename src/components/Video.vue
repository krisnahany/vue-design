<template>
    <div class="row">
        <div class="col-9 wrapper">
            <div class="row">
                <div class="col-3 border video-item" v-for="(obj, index) in listJSON" :key="index">
                    <img :src="obj.img" :alt="obj.alt">
                    <p class="participant-name">{{ obj.nama }}</p>
                </div>
            </div>
            <div class="button">
                <button><i class="fa fa-microphone-slash"></i></button>
                <button><i class="fa fa-video-camera"></i></button>
                <button><i class="fa fa-share-alt"></i></button>
                <button style="background-color:#00BCEB"><i class="fa fa-user-o"></i></button>
                <button><i class="fa fa-comment-o"></i></button>
                <button><i class="fa fa-ellipsis-h"></i></button>
                <button style="background-color:#F74B41"><i class="fa fa-times"></i></button>
            </div>
        </div>
        <participant :participant_list="listJSON"></participant>
    </div>
</template>

<script>
import Participant from './Participant'
export default {
    name: 'Video',
    components:{
        Participant
    },
    data: () => ({
        listJSON: [
            {
                img: require('../assets/img/boy1.jpg'),
                alt: 'Gwion John',
                nama: 'Gwion John'
            },
            {
                img: require('../assets/img/boy2.jpg'),
                alt: 'Alyx Greene',
                nama: 'Alyx Greene'
            },
            {
                img: require('../assets/img/girl1.jpg'),
                alt: 'Romany Tanner',
                nama: 'Romany Tanner'
            },
            {
                img: require('../assets/img/girl2.jpg'),
                alt: 'Maksymilian Stacey',
                nama: 'Maksymilian Stacey'
            },
            {
                img: require('../assets/img/girl3.jpg'),
                alt: 'Hermione Schneider',
                nama: 'Hermione Schneider'
            },
            {
                img: require('../assets/img/boy4.jpg'),
                alt: 'Jonathan Jennings',
                nama: 'Jonathan Jennings'
            },
            {
                img: require('../assets/img/girl4.jpg'),
                alt: 'Lilah Nairn',
                nama: 'Lilah Nairn'
            },
            {
                img: require('../assets/img/boy5.jpg'),
                alt: 'Portia Ryan',
                nama: 'Portia Ryan'
            },
            {
                img: require('../assets/img/boy6.jpg'),
                alt: 'Shayne Delgado',
                nama: 'Shayne Delgado'
            },
            {
                img: require('../assets/img/girl5.jpg'),
                alt: 'Chiara Ho',
                nama: 'Chiara Ho'
            },
            {
                img: require('../assets/img/girl6.jpg'),
                alt: 'Elena Jacobs',
                nama: 'Elena Jacobs'
            },
            {
                img: require('../assets/img/boy3.jpg'),
                alt: 'Esmee Bradford',
                nama: 'Esmee Bradford'
            }
        ]
    }),
}
</script>

<style lang="css">

    .col-3.video-item {
        padding: 0;
    }
    
    .col-3.video-item img {
        width: 100%;
        height: 100%;
        cursor: pointer;
    }

    p.participant-name {
        position: absolute;
        bottom: 0;
        transform: translateY(60%);
        color: white;
        background-color: #292929;
        opacity: 0.7;
        padding: 0 20px;
    }

    .wrapper .button {
        position: absolute;
        left: 50%;
        bottom: 20px;
        transform: translateX(-50%);
        margin: 0 auto;
    }
    .wrapper .button button {
        background-color: #292929;
        opacity: 0.7;
        border: none;
        border-radius: 50%;
        color: white;
        padding: 12px 16px;
        margin: 0 5px;
        cursor: pointer;
    }
    .wrapper .button button:hover {
        background-color: #292929;
        opacity: 1;
    }

</style>