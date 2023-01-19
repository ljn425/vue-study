<template>
  <div>
    <!-- <MarkdownDisplay :markdown="'# Hello'"></MarkdownDisplay> -->
    <textarea name="" v-model="testData" cols="30" rows="10"></textarea>
    <MarkdownDisplay :markdown="setMsg"></MarkdownDisplay>
    <!-- <highlight-display :hia="setMsg">--</highlight-display> -->
  </div>
</template>

<script>
import MarkdownDisplay from './components/MarkdownDisplay.vue';
// import HighlightDisplay from './components/HighlightDisplay.vue';

export default {
  data() {
    return {
      testData: '',
    };
  },
  components: {
    MarkdownDisplay,
    // HighlightDisplay,
  },
  computed: {
    setMsg() {
      return this.testData;
    },
  },
};
</script>

<style></style>
