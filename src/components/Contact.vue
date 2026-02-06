<script lang="ts"></script>
<template>
    <section id="contact">
        <h1>Contact me:</h1>

        <form target="_blank" action="https://formsubmit.co/arkhentark@gmail.com" method="POST">
            <input type="text" name="name" class="form-control" placeholder="Name" required>
            <input type="email" name="email" class="form-control" placeholder="Email Address" required>
            <textarea placeholder="Your Message" class="form-control" name="message" cols="20" rows="10"
                required></textarea>
            <button type="submit" class="btn btn-lg btn-dark btn-block">Submit Form</button>
        </form>
    </section>
</template>
<style scoped lang="sass">
    form 
        width: 100%
        input
            width: 100%
            color: black
                        
        textarea
            resize: none
            width: 100%
            color: black

        button
            color: black
            width: 100%
            height: 2rem
                        
            

</style>