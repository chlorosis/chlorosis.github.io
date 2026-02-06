<script setup lang="ts">
import Footer from './components/Footer.vue';
import Intro from './components/Intro.vue';
import PortfolioItem from './components/Portfolio-Item.vue';
import Portfolio from './components/Portfolio.vue';
import Navbar from './components/Navbar.vue';
import About from './components/About.vue';
import Contact from './components/Contact.vue';
const portfolio_items = [
    { id: 1, splash: './assets/splash/radiostations.png', description: 'A browser for radiostations api by api.radio-browser.info.\n Made using Vue, IndexedDB.', link: 'https://chlorosis.github.io/radiostations' },
    { id: 3, splash: './assets/splash/landing.png', description: 'The site you are on right now!\n Made using Vue', link: '#' },
];

function getAssetUrl(path: string) {
    return new URL(path, import.meta.url).href

}
// for 




</script>

<template>
    <div class="flex-container">
        <Navbar></Navbar>
        <Intro></Intro>
        <About></About>
        <Portfolio>
            <PortfolioItem v-for="item, index in portfolio_items" :id="item.id" :splash="getAssetUrl(item.splash)"
                :description="item.description" :link="item.link" />
        </Portfolio>
        <Contact></Contact>
        <Footer></Footer>
    </div>
</template>

<style scoped lang="sass">
    section
        padding: 1.5rem 1.5rem 3rem
    section, footer
        position: relative
        border-top: 2px solid white

    section:nth-child(odd)::before, footer:nth-child(odd)::before
        content:""
        position: absolute
        left: 0%
        top: -5ch
        width: 2px
        height: 10ch
        background-color: white

    section:nth-child(even)::before, footer:nth-child(even)::before
        content:""
        position: absolute
        right: 0%
        top: -5ch
        width: 2px
        height: 10ch
        background-color: white

</style>