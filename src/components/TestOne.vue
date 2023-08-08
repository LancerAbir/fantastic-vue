<script setup>
import { onMounted, ref } from "vue";

const name = ref("Paklu");

let hori = "Hare Krishna";
let numberOfId = 2;
let h2 = "text-4xl";
const great = () => {
    console.log(`Hello ${name.value}`);
};

const dynamicClassAndId = {
    class: "text-8xl",
    id: "13",
};

// onMounted Event Listeners এটি সব কাজ সেস করে সবার শেষে output দিবে
onMounted(great);
</script>

<template>
    <div>
        <p>
            {{ hori }}<br />
            Lorem ipsum dolor sit am
        </p>
    </div>
    <div v-html="hori"></div>
    <input type="text" :id="numberOfId" />
    <p :class="h2">text</p>

    <h3 :="dynamicClassAndId">Dynamic Class And ID</h3>
</template>
