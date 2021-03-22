<template>
    <b-container class="d-flex justify-content-center">
        <b-card class="main">
            <h1>title</h1>
            <p>body</p>
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
.main {
    margin-top:5%;
    width: 90%;
}
</style>