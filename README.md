# d3vue: a D3 Plugin for VueJS

> D3 integration with Vue.js

![d3vue](https://user-images.githubusercontent.com/5210420/38121793-621f10e8-339f-11e8-9c96-ce0b6f2512b2.png)

d3vue is a plugin for VueJS 2 that allows you to take data from your Vue instance and bind that data to a D3 v4 data visualization.  d3vue uses the v4 merge syntax so when you can call the same function in your lifecycle events (i.e. mounted, beforeUpdate).  The function signature is:

```
this.$helpers.chart.barChart(this.$d3, this.dataSet, this.options);
```
- this.$d3 is a reference to the d3 instances
- this.dataSet is an array of objects from your instances
- this.options includes
  - options.selector: selector name to place the graph.
  - options.metric: value you are measuring.
  - options.dim: value you will be categorizing the data by.
  - options.width: width of the chart.
  - options.height: height of the chart.

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
