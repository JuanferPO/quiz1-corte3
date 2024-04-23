<template>
  <ion-checkbox v-bind="$attrs" :type="type" :id="id" :value="value" :disabled="disabled">{{ value }}</ion-checkbox>
</template>

<script lang="ts">
  import { IonCheckbox } from '@ionic/vue';
  import { defineComponent } from 'vue';

  export default defineComponent({
    components: { IonCheckbox },
  props: {
    type: String,
    id: {
      type: String,
      required: true
    },
    name: String,
    value: String,
    disabled: Boolean,
  }
});
</script>
  
<style scoped></style>