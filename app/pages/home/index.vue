<template>
    <b-container class="d-flex justify-content-center">
        <b-card>
            <div v-for="url in urls" :key="url">
                <div class="video">
                    <iframe width="560" height="315" :src="url" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                </div>
            </div>
        </b-card>
    </b-container>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
    data() {
        return {
            urls: []
        }
    }
})
</script>

<style>
.video {
    margin: 2em;
}
</style>