<template>
  <div>
    <input type="text" v-model="name"/>
    <p>私は{{ name }}です</p>
    <p v-once>{{ name }}は大変です。</p>
    <!-- v-onceをつけると反映されない -->
    <div v-html="htmlData"/>
    <!-- v-htmlをつけるとHTMLを挿入できる -->

  </div>
</template>

<script>
export default {
  data() {
    return {
      name: 'エンジニア',
      htmlData: `<b><font color="red">私の名前はエンジニアです</font></b>`
      // HTML挿入
    }
  }
}
</script>

<style>

</style>
