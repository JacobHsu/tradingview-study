# tradingview-study

[TradingView 中文开发文档](https://zlq4863947.gitbook.io/tradingview/home)

tradingview / [charting-library-examples](https://github.com/tradingview/charting-library-examples)

charting_library

[charting_library-master](https://github.com/linzhifen5/charting_library-master)  
charting_library  
datafeeds  

tradingview [Advanced Real-Time Chart Widget](https://www.tradingview.com/widget/advanced-chart/)

## vuejs

> * ../../public/charting_library in ./node_modules/cache-loader/dist/cjs.js??ref--12-0!./node_modules/@vue/cli-plugin-babel/node_modules/babel-loader/lib!./node_modules/cache-loader/dist/cjs.js??ref--0-0!./node_modules/vue-loader/lib??vue-loader-options!./src/components/TVChartContainer.vue?vue&type=script&lang=js&

文件中引用的文件找不到。確認文件的相對路徑是否正確，可以解決此問題

```js
// import { widget } from '../../public/charting_library';
import { widget } from '../../public/charting_library/charting_library.min.js';

 const tvWidget = new widget(widgetOptions);
    this.tvWidget = tvWidget;
```

[技術分析圖表](https://tw.tradingview.com/HTML5-stock-forex-bitcoin-charting-library/?feature=technical-analysis-charts) `charting_library` & `datafeeds` 取自
alokshakya / BitcoinEtheriumLivePricing [src/assets](https://github.com/alokshakya/BitcoinEtheriumLivePricing/tree/master/src/assets)

> Cannot read property 'UDFCompatibleDatafeed' of undefined in react-javascript [#92](https://github.com/tradingview/charting-library-examples/issues/92)

public/index.html

```html
<script src="<%= BASE_URL %>datafeeds/udf/dist/polyfills.js"></script>
<script src="<%= BASE_URL %>datafeeds/udf/dist/bundle.js"></script>
```

datafeeds包內需要有檔案
public\datafeeds\udf\dist\polyfills.js
public\datafeeds\udf\dist\bundle.js