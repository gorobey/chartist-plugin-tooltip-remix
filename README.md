This is a simple remixed version of tooltip plugin for chartist (https://gionkunz.github.io/chartist-js/).

Removed "meta" from label, replaced from "name".

howto use:

```javascript
new Chartist.Line('.ct-chart', {
	labels: ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday'],
	series: [{
		name: 'Unique Users', //name of array data, visible in tootip
		data: [10, 15, 7, 18, 9],
	}, {
		name: 'Pages view', //name of array data, visible in tootip
		data: [32, 24, 16, 45, 12]
	}]
}, {
	high: 45,
	low: 0,
	position: 'start',
	showArea: false,
	fullWidth: true,
	distributeSeries: true,
	plugins: [
	Chartist.plugins.tooltip()
	],
	axisY: {
		onlyInteger: true
	}
  }
});
```


For Original plugin version visit:
https://github.com/Globegitter/chartist-plugin-tooltip

