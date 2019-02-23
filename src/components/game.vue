<template>
    <div class="game-container">
        <canvas ref="gameArea"></canvas>
    </div>
</template>

<script>
export default {
    name: 'game',
    data() {
        return {
            gameArea: '',
            gameCanvasContext: '',
        }
    },
    methods: {
        setupGamingArea() {
            this.gameArea = this.$refs.gameArea;
            this.gameCanvasContext = this.gameArea.getContext('2d');
        }
    },
    mounted() {
        this.setupGamingArea();
    },
}
</script>

<style>

</style>

