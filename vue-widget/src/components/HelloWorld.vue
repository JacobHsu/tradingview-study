<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <div id="tradingview_2536e"></div>
  </div>
</template>

<script>
import { onMounted } from 'vue';
export default {
  name: 'HelloWorld',
  props: {
    msg: String,
  },
  setup() {
    // mounted
    onMounted(() => {
      const widgetOptions = {
        width: 650,
        height: 400,
        symbol: 'AMEX:ARKK',
        interval: '60',
        timezone: 'Etc/UTC',
        theme: 'dark',
        style: '1',
        locale: 'zh_TW',
        toolbar_bg: '#f1f3f6',
        enable_publishing: false,
        allow_symbol_change: true,
        container_id: 'tradingview_2536e',
        // hide_top_toolbar: true,
        withdateranges: true,
        save_image: false,
        studies: ['DoubleEMA@tv-basicstudies', 'hullMA@tv-basicstudies'],
      };
      new window.TradingView.widget(widgetOptions);
    });
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
