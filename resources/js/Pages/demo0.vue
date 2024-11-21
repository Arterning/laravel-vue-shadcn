<script setup lang="ts">
import { Head, Link } from '@inertiajs/vue3';
import Button from '@/components/ui/button/Button.vue';
import Input from '@/components/ui/input/Input.vue';
import Select from '@/Components/Select.vue';
import BillBoard from '@/Components/BillBoard.vue';

defineProps<{
    name?: string;
}>();

</script>

<template>
    <Head title="Welcome" />
    <Button>nice job</Button>
    <Input placeholder="o"/>

    {{ name }}

    <div class="bg-indigo-200 ronded">
        div field 骚气的紫色
    </div>
    <Select />
</template>
