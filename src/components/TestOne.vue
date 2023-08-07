<script setup>
import { onMounted, ref } from "vue";

const name = ref("Paklu");

const great = () => {
    console.log(`Hello ${name.value}`);
};

onMounted(great);
</script>

<template>
    <div>
        <p>
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quaerat ab
            accusamus, beatae fugit ipsa perspiciatis, recusandae reprehenderit
            tenetur inventore velit possimus pariatur sit nulla esse magnam
            expedita voluptate facere et?
        </p>
    </div>
</template>
