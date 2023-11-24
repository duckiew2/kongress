<script setup>
	const props = defineProps({
		list:Array
	})
</script>
<template>
  <table>
  <tr v-for="item in list">
	  <td>{{ item.time }}</td>
	  <td>{{ item.person }}</td>
	  <td>{{ item.name }}</td>
  </tr>
  </table>
</template>

<style>
th,td {
	text-align: left;
	padding: 10px;
}
tr:nth-child(even) {
	background-color: #f0f0f0;
}
</style>
