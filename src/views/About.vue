<script setup>
import { ref } from "vue";
import Typing from "@components/Typing.vue";

const step = ref(0);
</script>

<template>
    <div class="h-full w-full px-8 pt-8 sm:px-12 sm:pt-12 lg:px-16 lg:pt-16">
        <Typing
            v-if="step >= 0"
            @done="step++"
            text="About Me HI MY NAME IS HANK ,I am the predictor ,I can predicate what you are donig,you are see my page right,I am so awesome ,thank you to see this,wisely worlds!!!!!!!!!!!!!!!!!!S,you are been rick roll, lol lmao"
            class="mb-8 block text-2xl sm:text-3xl lg:text-4xl"
        />
        <img
            src="https://memeprod.ap-south-1.linodeobjects.com/user-template/e824f53652754e144e696c862203bf43.png"
            alt="cool"
        />
        <img src="https://i.imgur.com/XycRU8th.jpg" alt="cool" />

        <Typing v-if="step >= 1" @done="step++" text="Who am I?" />
    </div>
</template>
