<template>
  <div class="main">
    <!-- <sample :text="items[1].name"></sample> -->
{{items[1].name}}
  </div>
</template>

<script lang="ts">
    import { Component,  Vue } from 'vue-property-decorator';
    import sample from '../components/sample.vue'

    @Component({
        components: {
          sample
    },
    })
    export default class Home extends Vue {
      items: { name: string, address: string, quantity: number}[] =[
        {
          name: "鉛筆",
          address: "大阪",
          quantity: 0
        },
        {
          name: "ノート",
          address: "東京",
          quantity: 0
        },
        {
          name: "消しゴム",
          address: "ニューヨーク",
          quantity: 0
        }
      ];

      item: string = "テスト"
    }
</script>