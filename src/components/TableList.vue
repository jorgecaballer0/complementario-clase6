<template>
  <div class="overflow-x-auto relative flex flex-col gap-4 mx-12">
    <!-- TABLA 1 -->
    <table class="text-sm text-left text-gray-500 dark:text-gray-400">
      <thead
        class="text-xs text-gray-700 uppercase bg-gray-50 dark:bg-gray-700 dark:text-gray-400"
      >
        <tr>
          <th scope="col" class="py-3 px-6">Nombre</th>
          <th scope="col" class="py-3 px-6">Apellido</th>
          <th scope="col" class="py-3 px-6">DNI</th>
          <th scope="col" class="py-3 px-6">Profesión</th>
        </tr>
      </thead>
      <TableComponent1
        v-for="(persona, i) of arrayPersonas1"
        :key="i"
        :personas1="persona"
      />
    </table>

    <!-- TABLA 2 -->
    <table class="text-sm text-left text-gray-500 dark:text-gray-400">
      <thead
        class="text-xs text-gray-700 uppercase bg-red-50 dark:bg-gray-700 dark:text-gray-400"
      >
        <tr>
          <th scope="col" class="py-3 px-6">Nombre</th>
          <th scope="col" class="py-3 px-6">Apellido</th>
          <th scope="col" class="py-3 px-6">DNI</th>
          <th scope="col" class="py-3 px-6">Profesión</th>
        </tr>
      </thead>
      <TableComponent2
        v-for="(persona, i) of arrayPersonas2"
        :key="i"
        :personas2="persona"
      />
    </table>

    <!-- TABLA 3 -->
    <table class="text-sm text-left text-gray-500 dark:text-gray-400">
      <thead
        class="text-xs text-gray-700 uppercase bg-green-50 dark:bg-gray-700 dark:text-gray-400"
      >
        <tr>
          <th scope="col" class="py-3 px-6">Nombre</th>
          <th scope="col" class="py-3 px-6">Apellido</th>
          <th scope="col" class="py-3 px-6">DNI</th>
          <th scope="col" class="py-3 px-6">Profesión</th>
        </tr>
      </thead>
      <TableComponent3
        v-for="(persona, i) of arrayPersonas3"
        :key="i"
        :personas3="persona"
      />
    </table>
  </div>
</template>

<script>
import TableComponent1 from "./Table1.vue";
import TableComponent2 from "./Table2.vue";
import TableComponent3 from "./Table3.vue";

export default {
  name: "TableListComponent",
  components: {
    TableComponent1,
    TableComponent2,
    TableComponent3,
  },

  data() {
    return {
      arrayPersonas1: [
        {
          nombre: "Juan",
          apellido: "Perez",
          dni: "45324804",
          profesion: "Arquitecto",
        },
        {
          nombre: "Martin",
          apellido: "Gonzalez",
          dni: "32657891",
          profesion: "Programador",
        },
        {
          nombre: "Agustin",
          apellido: "Sosa",
          dni: "321645789",
          profesion: "Abogado",
        },
      ],
      arrayPersonas2: [
        {
          nombre: "Melanie",
          apellido: "Pereira",
          dni: "17896432",
          profesion: "Contadora",
        },
        {
          nombre: "Pepe",
          apellido: "Sanchez",
          dni: "37854129",
          profesion: "Cocinero",
        },
        {
          nombre: "Marta",
          apellido: "Correa",
          dni: "11879632",
          profesion: "Pastelera",
        },
      ],
      arrayPersonas3: [
        {
          nombre: "Jorge",
          apellido: "Caballero",
          dni: "123456789",
          profesion: "Desarrollador web",
        },
        {
          nombre: "Soledad",
          apellido: "Gutierrez",
          dni: "47654321",
          profesion: "Desempleada",
        },
        {
          nombre: "Franco",
          apellido: "Fernandez",
          dni: "65798213",
          profesion: "Ejecutivo",
        },
      ],
    };
  },
};
</script>
