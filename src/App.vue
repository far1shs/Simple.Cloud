<template>
  <div style="margin: -8px">
    <Menubar :model="items">
      <template #start>
        <h4 style="margin: 0">Simple Cloud</h4>
      </template>
      <template #end>
        <Button icon="pi pi-cog" text size="small"/>
      </template>
    </Menubar>
  </div>
</template>

<script setup>
import {ref} from "vue";

const items = ref([
  {
    label: "服务器"
  }, {
    label: "域名"
  }
]);
</script>