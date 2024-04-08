<template>
  <NButton v-bind="buttonProps">button</NButton>
  <NPagination v-bind="pagination" />
  <NDataTable :pagination="pagination" />
</template>

<script lang="ts" setup>
import { reactive } from "vue";
import { NButton, NPagination, NDataTable } from "naive-ui";
import type { PaginationProps, ButtonProps } from "naive-ui";

const buttonProps = reactive<ButtonProps>({});
const pagination = reactive<PaginationProps>({});
</script>
