<template>
    <div>
        <div>Stuff Component</div>
        <a
            v-for="(course, index) in arrayOfStuff"
            :href="course.link"
            :key="index"
            ><div>
                {{ course.name }}
            </div>
        </a>
    </div>
</template>

<script>
export default {
    data() {
        return {
            arrayOfStuff: [
                { name: "photography", link: "http://www.youtube.com" },
                { name: "math", link: "http://www.twitter.com" },
                { name: "physics", link: "http://www.google.com" },
                { name: "music", link: "http://www.spotify.com" },
            ],
        };
    },
};
</script>

<style>
</style>