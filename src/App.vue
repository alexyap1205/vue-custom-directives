<template>
    <div class="container">
        <div class="row">
            <div class="col-xs-12 col-sm-8 col-sm-offset-2 col-md-6 col-md-offset-3">
                <h1>Built-in directive</h1>
                <p v-text="'Testing v-text'"></p>
                <hr>
                <h1>Custom directive</h1>
                <p v-highlight:background.delayed="'red'">Highlighted</p>
                <hr>
                <button v-listen:click="clicked">Test</button>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        methods: {
            clicked() {
                alert('clicked');
            }
        }
    }
</script>

<style>
</style>
