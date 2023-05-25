<template>
    <h1 class="clock">{{ time }}</h1>
</template>

<script setup>
    import { ref } from 'vue'

    const getTime = () => {
    const date = new Date()
    let seconds = date.getSeconds();
        let minutes = date.getMinutes();
        let hour = date.getHours();
        const weekday = ["Sunday","Monday","Tuesday","Wednesday","Thursday","Friday","Saturday"];
        let dayweek = weekday[date.getDay()];
        let utc = date.toLocaleDateString('pt-BR')
        
        minutes = minutes > 9 ? minutes : '0' + minutes;
        hour = hour > 9 ? hour: '0' + hour
        seconds = seconds > 9 ? seconds: '0' + seconds
    return `${dayweek}, ${hour}:${minutes}:${seconds} | ${utc} `
    }
    const time = ref(getTime())
    setInterval(() => time.value = getTime(), 1000)

</script>

<style>
    .clock {
        color: var(--comment);
        font-size: medium;
    }
</style>