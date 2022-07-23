<template>
    <h1>Hi</h1>
</template>

<script setup>
// Using the experimental setup syntax:
// https://github.com/vuejs/rfcs/blob/script-setup-2/active-rfcs/0000-script-setup.md

import { ref, defineProps } from "vue";

const props = defineProps(["usersFromProps"]);

const usersFromApi = ref([]);

fetch("./api/users")
    .then((res) => res.json())
    .then((res) => (usersFromApi.value = res));

const onClick = () => alert("clicked");
</script>
