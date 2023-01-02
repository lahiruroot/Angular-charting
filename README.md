# Angular-charting
charting library in an Angular application

To use a charting library in an Angular application, you will need to install the library using npm and then import it into your Angular component or module where you want to use it.

For example, if you want to use the ngx-charts library, you can install it using npm by running the following command:

```bash
npm install @swimlane/ngx-charts --save
```

Then, in the Angular component or module where you want to use the chart, you will need to import the library and add it to the imports array of the @NgModule decorator. For example:

```bash

import { NgxChartsModule } from '@swimlane/ngx-charts';

@NgModule({
  imports: [
    NgxChartsModule
  ]
})
export class MyModule { }

```

Once the library is imported, you can use its components in your template to add a chart to your Angular application. For example:

```bash

<ngx-charts-line-chart
  [view]="view"
  [scheme]="colorScheme"
  [results]="data"
  [gradient]="gradient"
  [xAxis]="showXAxis"
  [yAxis]="showYAxis"
  [legend]="showLegend"
  [showXAxisLabel]="showXAxisLabel"
  [showYAxisLabel]="showYAxisLabel"
  [xAxisLabel]="xAxisLabel"
  [yAxisLabel]="yAxisLabel">
</ngx-charts-line-chart>

```

This will add a line chart to your application. You can customize the appearance and behavior of the chart by binding to input properties of the chart component. Consult the documentation of the charting library you are using for more information on the available input properties and other customization options.
