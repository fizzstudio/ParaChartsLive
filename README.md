# ParaChartsLive

Demo of ParaCharts Live Updates.

## What this shows

Demonstrates the speed, accuracy, and relevance of ParaCharts, through our live feed feature. By default, new semi-random numbers are generated and sent to ParaCharts every 500ms, and ParaCharts not only updates the chart, but detects trends and relationships in the data and generates a fresh, relevant, deterministic description every half-second.

Pressing the back and foward buttons sends a new data window to the chart every time, so you can see that given the same input, the same output is generated.

This makes ParaCharts a dependable alt text generation system on its own, or can serve as a prompt for an LLM to make an enhanced description with solid grounding on what can be said about the chart.

## Advanced Controls

The advanced controls let you change how quickly the data is updated, how quickly the lines in a multi-series chart converge, and whether the full caption is shown or just the concise caption (default for this demo).

_**Note:** ParaCharts can generate a fresh chart and description in less than 100ms on common hardware, but this is not showcased in this demo because the random value generation doesn't converge the values fast enough. For speeds like that, set the `step` to 25, and the bias for each line to around -5 and 5, respectively._

## Accessibility

This demo concentrates on speed, not accessibility. The live feed feature is still under active development, and doesn't yet provide a screen reader update for changes to the chart. Full live-feed accessibility is expected to be included in June 2026.

## Description richness

This set of features is still under active development, and is currently optimized for showing change over time for 2 data series as they diverge, stay steady, converge, or intersect. After an intersection, the description does not yet include information about the gap differences; this functionality is expected to be much richer by May 2026.
