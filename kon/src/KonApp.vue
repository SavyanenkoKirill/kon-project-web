<script setup lang="ts">
</script>

<template>
    <div class="circle">
        <div class="kon-label">KON</div>
    </div>
</template>

<style scoped>
.circle {
    border: 10px dashed red;
    height: 300px;
    width: 300px;
    border-radius: 50%;

    display: flex;
    align-items: center; 
    justify-content: center;

    /* transition-duration: 0.8s;
    transition-property: transform;
    animation:spin 3s linear reverse infinite; */
}

.kon-label {
    position: absolute;

    font-style: italic;
    font-size: 140px;
    font-family: 'Bebas Neue';
    color: whitesmoke;
    text-shadow: 0 0 10px black;
    /* -webkit-text-stroke: 1px black; */
    /* animation:spin 3s linear infinite; */
}

@keyframes spin { 100% { transform:rotate(360deg); } }

/* .circle:hover {
    transform: rotate(360deg);
} */
</style>