## @superset-ui/plugin-chart-plugin-legend

[![Version](https://img.shields.io/npm/v/@superset-ui/plugin-chart-plugin-legend.svg?style=flat-square)](https://www.npmjs.com/package/@superset-ui/plugin-chart-plugin-legend)

This plugin provides Plugin Legend for Superset.

### Usage

Configure `key`, which can be any `string`, and register the plugin. This `key` will be used to lookup this chart throughout the app.

```js
import PluginLegendChartPlugin from '@superset-ui/plugin-chart-plugin-legend';

new PluginLegendChartPlugin().configure({ key: 'plugin-legend' }).register();
```

Then use it via `SuperChart`. See [storybook](https://apache-superset.github.io/superset-ui/?selectedKind=plugin-chart-plugin-legend) for more details.

```js
<SuperChart
  chartType="plugin-legend"
  width={600}
  height={600}
  formData={...}
  queriesData={[{
    data: {...},
  }]}
/>
```

### File structure generated

```
├── package.json
├── README.md
├── tsconfig.json
├── src
│   ├── PluginLegend.tsx
│   ├── images
│   │   └── thumbnail.png
│   ├── index.ts
│   ├── plugin
│   │   ├── buildQuery.ts
│   │   ├── controlPanel.ts
│   │   ├── index.ts
│   │   └── transformProps.ts
│   └── types.ts
├── test
│   └── index.test.ts
└── types
    └── external.d.ts
```
