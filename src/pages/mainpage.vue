<template>
    <div class="row py-3">
        <div class="col">
            <h1>Новости</h1>
        </div>
    </div>
    <div class="row">
        <div class="col-lg-3 col-md-4 col-sm-6 col-12 mb-2" v-for="article in articles" :key="article.id">
            <a href="#" class="card text-decoration-none">
                <img :src="article.image" class="card-img-top" alt="...">
                <div class="card-body">
                    <h5 class="card-title">{{ article.title }}</h5>
                </div>
            </a>
        </div>
    </div>
    <div class="row">
        <div class="col-lg-3 col-md-4 col-sm-6 col-12 mb-2" v-for="article in articles" :key="article.id">
            <a href="#" class="card text-decoration-none">
                <img :src="article.image" class="card-img-top" alt="...">
                <div class="card-body">
                    <h5 class="card-title">{{ article.title }}</h5>
                </div>
            </a>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            articles: [
                {
                    id: 1,
                    title: 'новость номер 1',
                    image: "https://i.pinimg.com/originals/b6/fc/05/b6fc0514cabfa0f434278903084c594c.jpg"
                },
                {
                     id: 2,
                    title: 'новость номер 2',
                    image: "https://tse1.explicit.bing.net/th/id/OIP.pRImamJgvHaEN59uXLtnzgHaFj?rs=1&pid=ImgDetMain&o=7&rm=3"
                }
            ]
        }
    }
}
</script>

<style scoped>
.card img {
 height: 200px;

}
</style>