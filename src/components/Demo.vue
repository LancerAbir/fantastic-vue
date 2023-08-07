<script setup>
import { reactive } from "vue";

// let refNameD = ref("");

const oldname = reactive({
    name: "kobir",
    age: 50,
});

const nameChange = () => {
    oldname.name = "New Fata kesto Developer ";
};

// export default {
//     name: "Demo",
//     data() {
//         return {
//             msg: "who am I ?",
//         };
//     },

//     methods: {
//         nameChange() {
//             this.msg = "who are you ?";
//         },
//     },
// };
</script>

<template>
    <div>
        <h3 class="text-2xl text-blue-500">ami holo</h3>
        <h3 class="text-2xl text-red-500">
            ami holo {{ oldname.name || "robin" }}
        </h3>
        <h4>
            age calculator is
            {{ oldname.age === 50 ? "ok" : "not" }}
        </h4>
        <button @click="nameChange">click me</button>
    </div>
</template>
