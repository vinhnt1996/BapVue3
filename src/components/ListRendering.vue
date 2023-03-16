<template>
    <div>
        <h1>List Rendering with v-for</h1>
        <h2>List Courses</h2>
        <ul v-for="item in courses" v-bind:key="item">
            <li>{{ key }} {{ item }}</li>
        </ul>
        <h2 v-for="item in courses" :key="item">{{ item }}</h2>
        <h2>List Fullname</h2>
        <ul v-for="(user, index) in fullNames" :key="index">
            <li>{{ index }} -- {{ user.first }} {{ user.last }}</li>
        </ul>
        <h3>List phức tạp</h3>
        <div v-for="actor in actors" :key="actor">
            <h2>{{ actor.name }}</h2>
            <h3 v-for="movie in actor.movies" :key="movie">{{ movie }}</h3>
        </div>
        <h2 v-for="(value, key, index) in myInfo" :key="value">{{ index }} {{ key }} {{ value }}</h2>
    </div>
</template>
<script>
export default {
    namne: 'ListRendering',
    data() {
        return {
            courses: [
                'Java',
                'HTML',
                'CSS',
                'PHP'
            ],
            fullNames: [
                { first: 'Bruce', last: 'Wayne'},
                { first: 'Clark', last: 'Kent'},
                { first: 'Princess', last: 'Diane'}
            ],
            actors: [
                {
                    name: 'Christian Bale',
                    movies: ['Batman', 'The Prestige']
                },
                {
                    name: 'Di Caprio',
                    movies: ['Titanic', 'Inception']
                }
            ],
            myInfo: {
                name: 'Vishwas',
                channel: 'Codevolution',
                course: 'Vue3'
            }
        }
    }
}
</script>
<style>
    
</style>