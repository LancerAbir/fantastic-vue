<script setup>
import { reactive, ref } from "vue";

// let refNameD = ref("");

const oldname = reactive({
    name: "kobir",
    age: 50,
});

let count = ref("50");

const nameChange = () => {
    oldname.name = "New Fata kesto Developer ";
};

// async function increment() {
//     count.value++;
//     await nextTick();
//     // Now the DOM is updated
// }
</script>

<template>
    <div>
        {{ count.value }}
        <h3 class="text-2xl text-blue-500">ami holo</h3>
        <h3 class="text-2xl text-red-500">
            ami holo {{ oldname.name || "robin" }}
        </h3>
        <h4>
            age calculator is
            {{ oldname.age === 50 ? "ok" : "not" }}
        </h4>
        <button @click="nameChange">click me</button> <br />

        <!-- <button @click="increment">click me</button> -->
    </div>
</template>
