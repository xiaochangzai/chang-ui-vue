<script>
import Vue from 'vue';
import { ChangUiSample, ChgButton, ChgNav } from '@/entry';

export default Vue.extend({
  name: 'ServeDev',
  components: {
    ChangUiSample,
    ChgButton,
    ChgNav
  }
});
</script>

<template>
  <div id="app">
    <ChgNav title="这是标题" url="http://123.345.com" linkText="蹦哒"/>
    <chang-ui-sample />
    <chg-button type='primary'><span>糖宝宝</span></chg-button>
  </div>
</template>
