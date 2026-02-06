<script setup lang="ts">


const props = defineProps<{
    id: number,
    splash: string,
    description: string,
    link: string
}>();

</script>

<template>
    <div class="item">
        <a :href="link" target="_blank" rek="noopener noreferrer">
            <div class="splash">
                <img :src="splash"></img>
            </div>
            <div class="description">{{ description }}</div>
        </a>
    </div>
</template>

<style lang="sass" scoped>

    .item

        width: 100%
        overflow: hidden
        margin: 0rem 1rem 1rem
        border: 3px solid #232323
        // box-shadow: 0px 0px 2px 1px  #8b8b8b
        

    .splash
        // overflow: hidden

        width: 100%
    
    .description
        text-align: center
        padding: 0rem 0.5rem 0.5rem
        white-space: preserve 
        word-break: keep-all
        background-color: #232323


    img
        
        object-fit: cover
        max-width: 100%
        


</style>