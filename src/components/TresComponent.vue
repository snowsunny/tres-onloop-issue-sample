<template>
<TresMesh>
  <TresTorusGeometry :args="[1, 0.5, 16, 32]" />
  <TresMeshBasicMaterial :color="color" />
</TresMesh>
</template>


<script>
import { useRenderLoop } from '@tresjs/core'

export default {
  name: 'TresComponent',
  props: {
    color: String
  },
  setup(props) {
    const { onLoop } = useRenderLoop()
    onLoop(() => {
      console.log('in onLoop   props:', props.color)
    })
  }
}
</script>