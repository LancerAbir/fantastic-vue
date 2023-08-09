<script setup>
import { reactive, ref } from "vue";

let number = ref(1);
let number2 = reactive(1);

const updateNumber = setInterval(() => {
    number.value++;
    number2++;
    student.name = "Tabbir";
    student.age = "52";
    student.batch = "5";
    student.subject = "Laravel, Node JS";
}, 3000);

const student = reactive({
    name: "Sabbir",
    age: 25,
    batch: 2,
    subject: "Vue, React",
});

console.log(updateNumber);
</script>

<template>
    {{ number }} <br />
    {{ number2 }} <br />

    {{ student.name }}
    {{ student.age }}
    {{ student.batch }}
    {{ student.subject }}
    <div>this is Count Components</div>

    <p>
        Lorem ipsum, dolor sit amet consectetur adipisicing elit. Reiciendis
        quae sequi nostrum? Consequuntur sequi minus eligendi? Quod similique
        architecto assumenda reprehenderit unde cum molestias illum beatae id
        aut ipsam voluptatem nisi dolorem sint minima, odio accusamus nobis.
        Quisquam, corrupti voluptatem, commodi, illo officia maxime id vitae
        dignissimos in eaque aliquid?
    </p>
</template>
