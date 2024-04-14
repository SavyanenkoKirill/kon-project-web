<script setup lang="ts">
</script>

<template>
    <div class="main">
        <!-- <div>Bla</div> -->
        <div class="circle">
            <div class="kon-label">KON</div>
        </div>
    </div>
</template>

<style scoped>
.main {
    /* display: flex;
  justify-content: center;
  align-items: center; */

  position: fixed;
  inset: 0px;
  width: 20rem;
  height: 20rem;
  margin: auto
}

.circle {
    /* border: 10px dashed; */
    /* border-style:groove; */


    height: 300px;
    width: 300px;
    border-radius: 50%;
    box-shadow: 0 0 100px rgb(31, 165, 255);

    display: flex;
    align-items: center; 
    justify-content: center;

    transition-duration: 0.8s;
    transition-property: transform;
    animation:spin 2s linear reverse infinite, pop linear 0.3s reverse, pulse 1.3s infinite;
}

.kon-label {
    position: absolute;

    font-style: italic;
    padding-right: 15px;

    font-size: 140px;
    font-family: 'Bebas Neue';
    color: rgb(31, 165, 255);
    text-shadow: 0 0 10px rgb(31, 165, 255);
    /* -webkit-text-stroke: 1px black; */
    /* animation:spin 3s linear infinite; */
}

/* @keyframes spin { 100% { transform:rotate(360deg);} } */
/* @keyframes pop { 100% {transform:scale(2, 2);}} */
@keyframes pulse {50% {transform: scale(1.2);} 100% {transform: scale(1);}}

/* .circle:hover {
    transform: rotate(360deg);
} */
</style>