<script setup lang="ts">
import { Head, Link } from '@inertiajs/vue3';
import Button from '@/components/ui/button/Button.vue';
import Input from '@/components/ui/input/Input.vue';
import Select from '@/Components/Select.vue';
import BillBoard from '@/Components/BillBoard.vue';
import CardList from '@/Components/CardList.vue';
defineProps<{
    name?: string;
}>();

</script>

<template>
    <Head title="Welcome" />
    <div class="bg-black">
        <BillBoard />
        <CardList />
    </div>
</template>
