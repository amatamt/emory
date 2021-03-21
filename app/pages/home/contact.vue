<template>
  <div>
      <InputName />
      <button @click="onSubmit">送信</button>
  </div>
</template>

<script lang="ts">
import Vue, { VueConstructor} from 'vue'
import InputName from '~/components/InputName.vue'

type State = {
  name: string
}

export default (Vue as VueConstructor<Vue & State>).extend({
  components: {
    InputName,
  },
  asyncData() {
    return {
      name: ''
    }
  },
  methods: {
    onSubmit() {
      const name = this.name
      alert(name)
    }
  }
})
</script>