<script setup>
import { usePage } from "@inertiajs/inertia-vue3";
const { props } = usePage();
</script>

<script>
export default { layoutName: "Narrow" };
</script>

<template>
    <div class="space-y-4">
        <h1 class="text-6xl">About Page</h1>
    </div>
</template>
