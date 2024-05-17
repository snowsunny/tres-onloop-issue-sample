<template>
  <div style="width: 500px; height: 500px">
   <TresCanvas>
     <TresPerspectiveCamera />
     <TresComponent color="green" />
   </TresCanvas>
  </div>
 </template>
 
 <script>
 import { TresCanvas, TresPerspectiveCamera } from '@tresjs/core';
 import TresComponent from './TresComponent.vue';
 export default {
   name: 'SecondPage',
   components: {
     TresCanvas, TresPerspectiveCamera, TresComponent
   }
 }
 </script>
 