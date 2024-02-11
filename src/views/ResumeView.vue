<script setup lang="ts">

import pdf from "../assets/tempRes.pdf";


</script>
<template lang="">
    <div class="wrapper">
        <embed class="resume" :src="pdf" />
    </div>
</template>

<style scoped>
    
    .wrapper {
        height: 100vh;
        width: 100vw;

    }
    .resume {
        height: 90%;
        width: 60%;
        /* make a media query for smaller screens to shrink pdf */
        zoom: 100%;
    }
</style>