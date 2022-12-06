<template>
  <div id="app" class="text-center mx-auto">
    <h1 class="text-center underline text-3xl font-bold m-4">
      Desafío complementario - Clase 6
    </h1>
    <TableListComponent />
  </div>
</template>

<script>
import TableListComponent from "./components/TableList.vue";

export default {
  name: "App",
  components: {
    TableListComponent,
  },
};
</script>
