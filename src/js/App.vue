<template>
    <div class="wrapper">
        <Nav />
        <div class="container">
            
            <Head />   
            
            <PopularArticle /> 
            <LastPublished /> 
            <Courses />
            <Info />
        </div>
    </div>
</template>

<script>
import Head from './components/Head.vue'
import Nav from './components/Nav.vue'
import PopularArticle from './components/PopularArticle.vue'
import LastPublished from './components/LastPublished.vue'
import Courses from './components/Courses.vue'
import Info from './components/Info.vue'
export default {
    components: {Head, Nav, PopularArticle, LastPublished, Courses, Info },
    
}
</script>

<style lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Roboto+Slab:wght@100;200;300;400;500;600;700;800;900&display=swap');
*{
    margin: 0;
    padding: 0;
}

body {
    background: #fff;
    color: #969393;
    font-family: 'Roboto Slab', serif;
    font-weight: 400;
    font-size: 1em;
    &::scrollbar {
            width: 8px;
        }
        
        &::-webkit-scrollbar {
            width: 8px;
        }

        &::-webkit-scrollbar-thumb {
            background-color: #c4c4c4;
            border-radius: 4px;
        }

        &::-webkit-scrollbar-thumb:hover {
            background-color: #a0a0a0;
        }

        &::-webkit-scrollbar-button {
            display: none;
        }
}
a {
    color: #ABABAB;
    text-decoration: none;
    &:hover {
        color: #c7c7c7
    }
}

.wrapper {
    overflow: hidden;
    
}


.container {

@media(min-width: 1500px){
    width: 1360px;
    margin: 0 auto;
}
@media(max-width: 1500px) and (min-width: 900px){
    width: 80%;
    margin: 0 10%;
}
@media(max-width: 900px){
    width: 90%;
    margin: 0 5%;
}
}

</style>