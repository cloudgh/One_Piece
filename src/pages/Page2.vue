<template>
    <div class="page2">
        <my-header></my-header>
        <div class="content">
            <iframe class="video"
                    src="https://www.youtube-nocookie.com/embed/Ades3pQbeh8?si=00016eJmrLF5oQiY" 
                    title="YouTube video player" 
                    frameborder="0" 
                    allow="accelerometer; autoplay; clipboard-write; 
                           encrypted-media; gyroscope; picture-in-picture; web-share" 
                    allowfullscreen></iframe>
            <p>
                Тизер-трейлер появился в сети 18 июня 2023 года. За 3 месяца он набрал 12 миллионов просмотров.
                Трейлер на этой странице был выложен на YouTube 22 июля 2023 года. Он набрал 12 миллионов просмотров уже за 2 месяца.
            </p>
        </div>
    </div>
</template>

<script>
import MyHeader from '@/components/MyHeader.vue';
export default {
    components:{
        MyHeader
    },
}
</script>

<style lang="scss" scoped>
.page2{
    font-family: 'Overpass', sans-serif;
    background: #ffa03acc;
    min-height: 100vh;
}

.content {
    display: flex;
    align-items: center;

    flex-direction: column;

    p {
        margin: 0 20vw;
        color: #f0ebeb;
        text-shadow: 2px 5px 4px #ffffff;
        backdrop-filter: blur;
    }
}

.video {
    border-radius: 4px;
    min-width: 70vw;
    min-height: 70vh;
    margin: 20px;
    box-shadow: 10px 20px 10px rgb(255, 120, 24),
                -50px 60px 10px rgba(255, 174, 0, 0.747),
                70px 80px 10px rgba(236, 30, 30, 0.836),
    ;
}
</style>