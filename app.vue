<template>
  <div>
    <div class="resources-data-table">
      <DataTable
        :value="value"
        :paginator="true"
        :rows="5"
        :rows-per-page-options="[5, 10, 20, 50]"
      >
        <Column field="name" header="Name"></Column>
        <Column field="surname" header="Surname"></Column>
        <Column field="phone" header="Phone"></Column>
        <Column field="email" header="Email"></Column>
      </DataTable>
    </div>
  </div>
</template>

<script setup lang="ts">
const value = [
  {
    name: "Albert",
    surname: "Hammond",
    phone: "3412341234",
    email: "ahammond@me.com",
  },
  {
    name: "Robert",
    surname: "Leslie",
    phone: "5436273537",
    email: "rleslie@me.com",
  },
];
</script>

<style></style>
