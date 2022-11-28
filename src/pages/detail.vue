<template>
    <div>
        <h1>This is Detail Page</h1>
        <h2>{{ subtitle }}</h2>
    </div>
</template>

<script>
export default {
  layout: "original",
  data() {
    return {
      subtitle: 'この文書はNuxt.jsの基本的な使用方法について説明しています。'
    }
  }
};
</script>