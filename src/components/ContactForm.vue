<template>
    <form action="https://api.web3forms.com/submit" method="POST" ref="contact" >

    <input type="hidden" name="access_key" value="fd5c0c6a-3714-48ae-a07a-3003966b55b4">

    <input type="text" name="name" placeholder="Your Name" v-model="userName" required class="contact">
    <br>
    <input type="email" name="email" placeholder="Your Email" v-model="userEmail" required class="contact">
    <br>
    <br>
    <textarea name="message" placeholder="What would you like to say?" v-model="message" required id="messageBox"></textarea>
    <input type="hidden" name="redirect" value="https://web3forms.com/success">
    <br>
    <button type="submit">Submit Form</button>

    </form>
</template>

<script lang="ts">

export default {
    data() {
        return {
            userName: '',
            userEmail: '',
            message: ''
        }
    }
};

</script>

<style>
    #messageBox {
        width: 500px;
        height: 150px;
    }
    .contact {
        width: 250px;
    }
</style>