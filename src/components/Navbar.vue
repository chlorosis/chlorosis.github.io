<script lang="ts">
</script>

<template>
    <nav>
        <div class="nav-link"><a href="#about">About me</a></div>
        <div class="nav-link"><a href="#portfolio">My work</a></div>
        <div class="nav-link"><a href="#contact">Contact</a></div>
    </nav>
</template>

<style lang="sass" scoped>

    nav
        display: flex
        justify-content: end

    .nav-link
        border-right: 2px solid white
        padding: 0 1ch
        background-color: none
        transition: 0.3s all


    
    .nav-link:last-of-type
        border: none

    .nav-link:hover
        background-color: var(--font-color)
        color: var(--secondary-color)
        transition: 0.3s all


</style>