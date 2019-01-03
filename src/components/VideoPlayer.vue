<template>
    <div class="video__player">
        <div class="video__list">
            <div :key="video.id" v-for="video in videos" class="thumbnail">
                <div class="thumbnail-img">
                    <img :src="video.thumbnail" />
                </div>
                <div class="thumbnail-info">
                    <h3>{{video.title}}</h3>
                    <p>{{video.creator}}</p>
                    <p class="thumbnail-views">{{video.views}} Views</p>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
let videos = [{
        id: 1,
        title:'Macie Jay Thermite',
        thumbnail: 'https://img.youtube.com/vi/HRdeN5tTHBk/0.jpg',
        youtubeURL: 'https://www.youtube.com/watch?v=HRdeN5tTHBk',
        creator: 'Macie Jay',
        likes: 0,
        views: 0
    },
    {
        id: 2,
        title:'Zakk Wylde',
        thumbnail: 'https://img.youtube.com/vi/TgPhUNZ3db4/0.jpg',
        youtubeURL: 'https://www.youtube.com/watch?v=TgPhUNZ3db4',
        creator: 'Zakk Wylde',
        likes: 0,
        views: 0 
    },
    {
        id: 3,
        title:'Linus Laptop',
        thumbnail: 'https://img.youtube.com/vi/RaLMgJA1HKc/0.jpg',
        youtubeURL: 'https://www.youtube.com/watch?v=RaLMgJA1HKc',
        creator: 'Linus Tech Tips',
        likes: 0,
        views: 0 
    },
    {
        id: 4,
        title:'Razer Headset',
        thumbnail: 'https://i.ytimg.com/vi/DvnSRj8xQBI/hqdefault.jpg?sqp=-oaymwEZCNACELwBSFXyq4qpAwsIARUAAIhCGAFwAQ==&rs=AOn4CLAsdihH_sWaTJpIC7M2fX94wFBRag',
        youtubeURL: 'https://www.youtube.com/watch?v=DvnSRj8xQBI&t=297s',
        creator: 'Linus Tech Tips',
        likes: 0,
        views: 0 
    },
    {
        id: 5,
        title:'Metallica Guitar Talk with James',
        thumbnail: 'https://i.ytimg.com/an_webp/nKHAQSyMTMo/mqdefault_6s.webp?du=3000&sqp=CNyDuOEF&rs=AOn4CLCsB0dGcUb1BmQL4pMO2uZoeRsCyQ',
        youtubeURL: 'https://www.youtube.com/watch?v=nKHAQSyMTMo',
        creator: 'Metallica TV',
        likes: 0,
        views: 0 
    },
    {
        id: 6,
        title:'Metallica: Orion live 2018',
        thumbnail: 'https://img.youtube.com/vi/iL42fwM5muE/0.jpg',
        youtubeURL: 'https://youtu.be/iL42fwM5muE',
        creator: 'Metallica TV',
        likes: 0,
        views: 0 
    }];
export default {
    name: 'VideoPlayer',
    data () {
        return {
            videos
        }
    }
}
</script>

<style>

</style>
