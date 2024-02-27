<template>
    <div class="page3">
        <my-header></my-header>
        <div class="content">
            <p>Рекламные постеры с актерами сериала One Piece от Netflix</p>
            <div class="images-grid">
                <img src="@/assets/wanted0.png" alt="">
                <img src="@/assets/wanted1.png" alt="">
                <img src="@/assets/wanted2.png" alt="">
            </div>
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
.page3{
    font-family: 'Overpass', sans-serif;

    background: 
        radial-gradient(circle at 36% 65%,
                        rgba(202, 188, 188, 0.808) 2%,
                        transparent 18% 
        ),
        radial-gradient(circle at 43% 57%,
                        rgba(202, 188, 188, 0.808) 5%,
                        rgb(255, 238, 0) 7%,
                        transparent 9% 
        ),
        radial-gradient(circle ,
                        rgba(224, 0, 0, 0.808) 10%,
                        rgba(255, 255, 0, 0.863) 70%,
                        #d12d2de8 90%,
        ),
    ;
    min-height: 100vh;
}

.content {
    display: flex;
    flex-direction: column;
    align-items: center;

    p {
        font-size: 20px;
        margin-top: 40px;
        margin-bottom: 20px;
        text-shadow: 1px 4px 5px #493636ee;
        background-color: rgba(231, 214, 182, 0.747);
        border-radius: 4px;
        padding: 5px;
    }
}
.images-grid {
    display: flex;
    justify-content: space-between;
    width: 90vw;
    img {
        max-width: 25vw;
        border-radius: 2px;
        box-shadow: 0px
                    30px
                    30px 
                    rgba(0, 0, 0, 0.808);
    }
}
</style>