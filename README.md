# iris: a bird's-eye view of variant annotations

<a href="https://stanfordbioinformatics.github.io/iris"><img src="https://stanfordbioinformatics.github.io/iris/preview2.png" width=800></a>

### About

How do we show a visual overview of variant annotations, when those annotations can come from anywhere and mean anything? When we don't even know how many annotation sources we're interested in?

Let's simplify. First, we know we want to draw things on a screen. That implies 2D space. So, let's just consider annotations that can be meaningfully mapped to a y-axis. That means we're only looking at ranked or quantitative data. 

Next, we don't know how many annotations we want to include, and we need room to show them. We haven't used our x-axis yet, so let's place each annotation's y-axis left to right, side by side.

Now, we can draw each variant as a line, going from left to right, connecting its corresponding points on each annotation axis.

This is called <a href="https://en.wikipedia.org/wiki/Parallel_coordinates">parallel coordinates</a>. It's good at showing relationships in multidimensional data. We want to try using it to show variant annotations.

### Sources
- D3 Javascript visualization library: https://d3js.org
- Parallel coordinates with reorderable axes: https://bl.ocks.org/jasondavies/1341281
- CADD scores: http://cadd.gs.washington.edu
- ExAC exomes: http://exac.broadinstitute.org
