<template>
  <tbody>
    <tr class="bg-green-400 border-b dark:bg-gray-800 dark:border-green-700">
      <th
        scope="row"
        class="py-4 px-6 font-medium text-gray-900 whitespace-nowrap dark:text-white"
      >
        {{ personas3.nombre }}
      </th>
      <td class="py-4 px-6 text-gray-900 dark:text-white">
        {{ personas3.apellido }}
      </td>
      <td class="py-4 px-6 text-gray-900 dark:text-white">
        {{ personas3.dni }}
      </td>
      <td class="py-4 px-6 text-gray-900 dark:text-white">
        {{ personas3.profesion }}
      </td>
    </tr>
  </tbody>
</template>

<script>
export default {
  name: "TableComponent3",

  props: {
    personas3: Object,
  },
};
</script>
