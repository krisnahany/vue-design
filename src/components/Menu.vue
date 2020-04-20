<template>
    <div class="menu">
        <div class="title-app">
            <img class="logo left" src="../assets/img/emoji.svg" alt="">
            <p class="left">Online Meetings</p>
            <div class="window right">
                <button><i class="fa fa-window-minimize"></i></button>
                <button><i class="fa fa-window-restore"></i></button>
                <button><i class="fa fa-times"></i></button>
            </div>
            <div class="clearfix"></div>
        </div>
        <nav class="navbar navbar-expand-lg navbar-light bg-light reset">
            <div class="collapse navbar-collapse">
                <ul class="navbar-nav mr-auto">
                    <li class="nav-item">
                        <a class="nav-link" href="#">File<span class="sr-only">(current)</span></a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Edit</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Share</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">View</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Audio</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Participant</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Meeting</a>
                    </li>
                    <li class="nav-item">
                        <a class="nav-link" href="#">Help</a>
                    </li>
                </ul>
                <p>Connected</p>
                <i class="fa fa-circle"></i>
            </div>
        </nav>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="css">
    .menu .title-app {
        padding: 0;
        margin: 0;
    }

    .menu .title-app .logo {
        margin: 5px 0;
        height: 20px;
        width: 20px;
    }

    .menu .title-app p {
        margin: 0;
        padding: 5px;
    }

    .menu .title-app .window {
        margin: 0;
    }

    .menu .title-app .window button i{
        font-size: 0.73em;
        margin-left: 10px;
    }
    
    .menu nav {
        padding: 0;
    }

    .menu nav p::before {
        content: '|';
        margin: 0 8px;
    }

    .menu nav p {
        font-size: 0.75em;
        margin: 0;
    }

    .menu nav i{
        padding: 0 5px;
        font-size: 0.55em;
        color: #00BCEB;
    }

    .menu nav ul li a {
        font-size: 0.75em;
    }
</style>