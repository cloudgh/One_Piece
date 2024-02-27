<template>
    <div class="page1">
        <my-header></my-header>
        <div class="content">
            <a href="https://www.kinopoisk.ru/series/1346615/?utm_referrer=yandex.ru">
                <img class="poster" src="@/assets/poster0.jpg" alt="">
            </a>
            <div class="description">
                <h1>One Piece</h1>
                <h3>Сериал 2023г</h3>
                <p class="first">Главный герой этой истории - парень в соломенной шляпе по имени Монки Д. Луффи. Все о чем мечтает наш герой - это приключения и путешествия. Будучи маленьким ребенком, он съедает дьявольский фрукт и становится резиновым человеком. Теперь у него есть необычная способность - он может растягивать свое тело и конечности до любых размеров. Сейчас перед Луффи стоит цель - стать главным среди пиратов. Но для этого, судя по легендам, необходимо добраться до древнего сокровища Ван Пис. Когда-то сам Гол Д. Роджер спрятал его где-то на Гранд Лайн, течении, которое объединяет множество островов по всему миру. Наш весельчак решает отправиться на их поиски.</p>
                <p class="second">Однако, наш персонаж далеко не единственный, кто охотится за золотом Роджера. Казалось бы, у нашего смышленого парня есть всё, для того чтобы стать королем - необычайная сила и острый ум. Не хватает только одного - верной и преданной команды, которые последуют за своим капитаном навстречу любой опасности. Вот только Луффи стоит поторопиться, ведь за Ван Пис идет целая ватага злобных пиратов, которая не остановится ни перед чем, чтобы добраться до заветного сокровища. Монки придется предпринять немало усилий, чтобы опередить всех своих соперников. </p>
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
.page1{
    background-image: url('@/assets/background40.png');
    min-height: 100vh;
}
h1 {
    color: rgb(231, 214, 182);
    max-width: max-content;
    font-family: 'ONE PIECE';
    font-size: 18vh;
    text-shadow: (5px 3px 4px rgb(59, 51, 47), 
                 25px 15px 8px rgba(148, 106, 8, 0.692));
    transition: 0.1s ease-in-out;
}
h1:hover {
    padding-left: 20px;
    transition: 0.1s ease-in-out;
}
.content {
    display: flex;
}

.description {
    font-family: 'Overpass', sans-serif;
    font-size: 20px;
    padding: 10px;
    color: #032e44;
    .first {
        text-shadow: 2px 1px 2px rgb(199, 199, 212);
    }
    .second{
        padding-top: 20px;
        color: #335464;
        text-shadow: 2px 1px 10px rgb(200, 200, 207);
    }
}

$poster-margin: 20px;
.poster {
    max-width: 30vw;
    max-height: 80vh;
    margin: $poster-margin;
    box-shadow: $poster-margin / 2
                $poster-margin / 1.5
                20px 
                rgb(0, 0, 0);
    border-radius: 4px;
    transition: 0.1s ease-out;
}
.poster:hover {
    margin-top: $poster-margin * 1.5;
    margin-right: $poster-margin / 2;
    margin-bottom: $poster-margin / 2;
    margin-left: $poster-margin * 1.5;
    box-shadow: $poster-margin / 2
                $poster-margin / 2 
                20px 
                rgb(0, 0, 0);
    transition: 0.1s ease-in;
}
</style>