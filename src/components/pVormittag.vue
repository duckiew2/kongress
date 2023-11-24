<script setup>
import { ref } from 'vue'
import ProgramComponent from '../components/ProgramComponent.vue'

const vortraege = ref([
	{time: '09:45', person: 'Max Riegel', name: 'Beginn und Einführung'},
	{time: '10:00', person: 'Joerg Kinzebach', name: 'Statische Webseiten'},
	{time: '11:00', person: 'Jochen Krapf', name: 'Altbewährtes Erbe'},
	{time: '12:00', person: '', name: '=== Mittagspause ==='}
])
</script>

<template>
  <div>
	  <h3>Vormittag</h3>
	  <ProgramComponent :list=vortraege />
  </div>
</template>

