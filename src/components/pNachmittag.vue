<script setup>
import { ref } from 'vue'
import ProgramComponent from '../components/ProgramComponent.vue'

const vortraege = ref([
	{time: '13:00', person: 'Martin Bokämper', name: 'Internet-Zugang über GSM, UMTS, LETE und 5G'},
	{time: '13:40', person: 'Herbert Oppmann', name: 'Ahnenforschung im Laufe der Zeit'},
	{time: '14:20', person: 'Matthias Brüstle', name: 'Der Microcontroller ESP 32'},
	{time: '15:00', person: '', name: '=== Kaffeepause ==='},
	{time: '15:30', person: 'Matthias Kirschner', name: 'Vorstellung Ada & Zangemann'},
	{time: '16:30', person: 'Hans-Jürgen Beie', name: 'Das Backup-Karussell dreht sich immer noch'},
	{time: '17:15', person: 'Andreas Merz', name: 'Gedanken zur Energiewende - Erfahrungen eines Prosumers'},
	{time: '17:30', person: '', name: 'Kongress Ausklang'}
])
</script>
<template>
  <div>
	  <h3>Nachmittag</h3>
	  <ProgramComponent :list=vortraege />
  </div>
</template>
