<template>
  <p>{{ text }}</p>
</template>

<script lang="ts">
import { Component, Prop,  Vue } from 'vue-property-decorator';

@Component
  export default class Home extends Vue {
    @Prop({ type: String, default: '' })
    text!: String
 }

</script>