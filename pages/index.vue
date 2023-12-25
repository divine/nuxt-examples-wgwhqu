<template>
  <div>
    Home
    <button @click="startLoading()">Start Loading Indicator</button>
  </div>
</template>
<script setup lang="ts">
const router = useRouter()

function startLoading(){
  useLoadingIndicator().start()
  console.log('Started loading indicator...')
}
</script>