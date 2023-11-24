<script setup>
    import { shallowRef } from 'vue'
    import pV from '../components/pVormittag.vue'
    import pN from '../components/pNachmittag.vue'

    const activeComponent = shallowRef(pV) 
</script>

<template>
  <div class="program">
    <h1>das Kongress Programm</h1>
	<label>
	    <input type="radio" v-model="activeComponent" :value="pV"> Vormittag
	</label>
	<label>
	    <input type="radio" v-model="activeComponent" :value="pN"> Nachmittag
	</label>
	<div class="programbox">
	    <Transition name="fade" mode="out-in">
	      <component :is="activeComponent"></component>
	    </Transition>
	</div>
  </div>
</template>

<style>
@media (min-width: 1024px) {
  .program {
    min-height: 100vh;
    display: flex;
    align-items: center;
  }
}

.programbox {
	padding-top: 10px;
	padding-left: 30px;
}

.fade-enter-active,
.fade-leave-active {
  transition: opacity 0.5s ease;
}

.fade-enter-from,
.fade-leave-to {
  opacity: 0;
}
</style>
