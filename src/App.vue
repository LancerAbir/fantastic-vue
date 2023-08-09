<script setup>
// import HelloWorld from "./components/HelloWorld.vue";
import { reactive, ref } from "vue";
import Count from "./components/Count.vue";
import Demo from "./components/Demo.vue";
import TestOne from "./components/TestOne.vue";
let refName = ref("");

const formFunction = reactive({
    reactiveName: "lancer",
});

const NameChangeHandler = () => {
    formFunction.reactiveName = "Vue Developer";
};

// console.log(refName.value);
// console.log(formFunction.reactiveName);
</script>

<template>
    <div>
        <h1 class="text-4xl font-bold underline-offset-8 text-black-500">
            Demo Components
        </h1>
        <Demo />

        <hr />
        <h1 class="text-4xl font-bold underline-offset-8 text-black-500">
            Test One Components
        </h1>
        <TestOne />
        <hr />
        <h1 class="text-4xl font-bold underline-offset-8 text-black-500">
            Count Components
        </h1>
        <Count />

        <hr />
        <h1 class="font-bold text-red-500">Hello, I am Lancer Abir</h1>
        <h2>ref - Name : {{ refName }}</h2>
        <input type="text" v-model="refName" />
        <hr />
        <h2>reactiveName - Name :{{ formFunction.reactiveName }}</h2>
        <input type="text" v-model="formFunction.reactiveName" />
        <hr />
        <button @click="NameChangeHandler">Name Change</button>
    </div>
</template>
