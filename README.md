# shared-assets
Host files that are used by multiple apps

## Notes about my modifications to plotly.js

Script source: local download of the plotly mapbox distribution.
It includes everything I need:
scatter, scattermapbox, choroplethmapbox and densitymapbox
https://github.com/plotly/plotly.js/blob/master/dist/README.md#partial-bundles

Since the script is in external_scripts and supplies the global Plotly var,
it is used over the other plotly packages by default.

Note: Local scripts are by default from `async-plotlyjs.js`, which is
minified and incomprehensible when debugging. Using plotly-mapbox,
for example, allows me to see what is going on for easier debugging
and future edits to the script itself.
https://community.plotly.com/t/smaller-version-of-async-plotlyjs-js-its-so-big-and-loads-so-slow/42247/2
https://github.com/plotly/dash-docs/issues/723#issuecomment-656393396
https://github.com/plotly/plotly.js/blob/master/dist/README.md#partial-bundles
