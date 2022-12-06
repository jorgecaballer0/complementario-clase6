<template>
  <tbody>
    <tr class="bg-red-400 border-b dark:bg-gray-800 dark:border-red-700">
      <th
        scope="row"
        class="py-4 px-6 font-medium text-gray-900 whitespace-nowrap dark:text-white"
      >
        {{ personas2.nombre }}
      </th>
      <td class="py-4 px-6 text-gray-900 dark:text-white">
        {{ personas2.apellido }}
      </td>
      <td class="py-4 px-6 text-gray-900 dark:text-white">
        {{ personas2.dni }}
      </td>
      <td class="py-4 px-6 text-gray-900 dark:text-white">
        {{ personas2.profesion }}
      </td>
    </tr>
  </tbody>
</template>

<script>
export default {
  name: "TableComponent2",

  props: {
    personas2: Object,
  },
};
</script>
