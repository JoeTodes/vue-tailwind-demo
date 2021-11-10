<template>
    <h1 class="text-center text-5xl font-bold bg-red-500">{{ count }}</h1>
    <button
        @click="incrementCount()"
        class="
            ml-48
            hover:bg-blue-300
            bg-gray-300
            border-2 border-black
            rounded-full
            px-2
        "
    >
        Click Me!
    </button>
    <ListOfStuff class="ml-28" />
</template>

<script>
import ListOfStuff from "./components/ListOfStuff.vue";

export default {
    data() {
        return {
            count: 0,
        };
    },
    components: { ListOfStuff },
    methods: {
        incrementCount() {
            this.count++;
        },
    },
};
</script>

<style>
</style>
