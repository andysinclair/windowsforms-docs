---
layout: post
title: Legend
description: This section describes about legend.
platform: windowsforms
control: SfSmithChart
documentation: ug
---
# Legend

Legend contains a list of chart series that appears in Smith chart. It can be defined by using the following code example.

To enable the legend for the Smith chart, set the [`Visible`](https://help.syncfusion.com/cr/cref_files/windowsforms/Syncfusion.SfSmithChart.WinForms~Syncfusion.WinForms.SmithChart.ChartLegend~Visible.html) property of legend to true.

{% tabs %}

{% highlight c# %}

chart.Legend.Visible = true;

{% endhighlight %}

{% highlight vb.net %}

chart.Legend.Visible = True

{% endhighlight %}

{% endtabs %}

Add name to the [`LegendText`](https://help.syncfusion.com/cr/cref_files/windowsforms/Syncfusion.SfSmithChart.WinForms~Syncfusion.WinForms.SmithChart.ChartSeries~LegendText.html) property of series, which in turn mapped to the legend.

{% tabs %}

{% highlight c# %}

series.LegendText = "Transmission1";

{% endhighlight %}

{% highlight vb.net %}

series.LegendText = "Transmission1"

{% endhighlight %}

{% endtabs %}

![C:/Users/yogapriya.shanmugam/AppData/Local/Microsoft/Windows/INetCacheContent.Word/legendScroll.png](Legend_images/Legend_img8.png)

## Positioning the legend

Legends can be docked at the left, right, and top or bottom around the chart area by using the [`DockPosition`](https://help.syncfusion.com/cr/cref_files/windowsforms/Syncfusion.SfSmithChart.WinForms~Syncfusion.WinForms.SmithChart.ChartLegend~DockPosition.html) property.

By default, the Smith chart’s legend is docked at the top of the chart. To display the legend at the bottom, set the [`DockPosition`](https://help.syncfusion.com/cr/cref_files/windowsforms/Syncfusion.SfSmithChart.WinForms~Syncfusion.WinForms.SmithChart.ChartLegend~DockPosition.html) property to Bottom as shown in the following code snippet.

![C:/Users/yogapriya.shanmugam/AppData/Local/Microsoft/Windows/INetCacheContent.Word/Dockbottom.png](Legend_images/Legend_img3.PNG)


## Legend icon

Represents the symbol associated with each legend item. By default, the legend icon is circle.

Legend icon can be customized by using the [`IconType`](https://help.syncfusion.com/cr/cref_files/windowsforms/Syncfusion.SfSmithChart.WinForms~Syncfusion.WinForms.SmithChart.ChartLegend~IconType.html) property in Smith chart’s legend as shown in the following code snippet.

{% tabs %}

{% highlight c# %}

sfSmithChart1.Legend.IconType = SmithChartLegendIconType.Rectangle;

{% endhighlight %}

{% highlight vb.net %}

sfSmithChart1.Legend.IconType = SmithChartLegendIconType.Rectangle

{% endhighlight %}

{% endtabs %}

![C:/Users/yogapriya.shanmugam/AppData/Local/Microsoft/Windows/INetCacheContent.Word/Icontype.png](Legend_images/Legend_img4.PNG)


## Legend alignment

The alignment of a legend can be changed to near, far, or center using the [`Alignment`](https://help.syncfusion.com/cr/cref_files/windowsforms/Syncfusion.SfSmithChart.WinForms~Syncfusion.WinForms.SmithChart.ChartLegend~Alignment.html) property.

By default, the legend is aligned to the center.

![C:/Users/yogapriya.shanmugam/AppData/Local/Microsoft/Windows/INetCacheContent.Word/LegendAlignment.png](Legend_images/Legend_img5.PNG)


## Customizing legend

Legend icon and text can be customized using the [`IconType`](https://help.syncfusion.com/cr/cref_files/windowsforms/Syncfusion.SfSmithChart.WinForms~Syncfusion.WinForms.SmithChart.ChartLegend~IconType.html), [`IconHeight`](https://help.syncfusion.com/cr/cref_files/windowsforms/Syncfusion.SfSmithChart.WinForms~Syncfusion.WinForms.SmithChart.ChartLegend~IconHeight.html), [`IconWidth`](https://help.syncfusion.com/cr/cref_files/windowsforms/Syncfusion.SfSmithChart.WinForms~Syncfusion.WinForms.SmithChart.ChartLegend~IconWidth.html) and [`ForeColor`](https://help.syncfusion.com/cr/cref_files/windowsforms/Syncfusion.SfSmithChart.WinForms~Syncfusion.WinForms.SmithChart.LegendStyle~ForeColor.html) properties.

The following code example illustrates the customization of legend icon and text.

{% tabs %}

{% highlight c# %}

sfSmithChart1.Legend.IconType = SmithChartLegendIconType.Pentagon;

sfSmithChart1.Legend.IconHeight = 13;

sfSmithChart1.Legend.IconWidth = 13;

sfSmithChart1.Legend.Style.ForeColor = Color.BlueViolet;

{% endhighlight %}

{% highlight vb.net %}

sfSmithChart1.Legend.IconType = SmithChartLegendIconType.Pentagon

sfSmithChart1.Legend.IconHeight = 13

sfSmithChart1.Legend.IconWidth = 13

sfSmithChart1.Legend.Style.ForeColor = Color.BlueViolet

{% endhighlight %}

{% endtabs %}

![C:/Users/yogapriya.shanmugam/AppData/Local/Microsoft/Windows/INetCacheContent.Word/LegendCustomize.png](Legend_images/Legend_img6.PNG)


## Toggle series visibility

Visibility of the series can be controlled by clicking the legend item. This can be done using the [`ToggleSeriesVisible`](https://help.syncfusion.com/cr/cref_files/windowsforms/Syncfusion.SfSmithChart.WinForms~Syncfusion.WinForms.SmithChart.ChartLegend~ToggleSeriesVisible.html) property.

{% tabs %}

{% highlight c# %}

sfSmithChart1.Legend.ToggleSeriesVisible = true;

{% endhighlight %}

{% highlight vb.net %}

sfSmithChart1.Legend.ToggleSeriesVisible = True

{% endhighlight %}

{% endtabs %}

![C:/Users/yogapriya.shanmugam/AppData/Local/Microsoft/Windows/INetCacheContent.Word/LegendToggle.png](Legend_images/Legend_img7.png)

## Smart view

### Scrollbar

Any number of series can be used in Smith chart. For each series, legend item will be displayed to indicate that series. If the chart area does not have enough space to accommodate all the legend items, then the scrollbar will be enabled automatically for visualizing all the legend items.

In the  following screenshot, around 7 series are added, and some of the series are defined with the same data points. Here, the specified dimension of chart can’t hold all the legend items in the view. Hence, the scroll bar is enabled for better visualization of legend items.

![C:/Users/yogapriya.shanmugam/AppData/Local/Microsoft/Windows/INetCacheContent.Word/legendScroll.png](Legend_images/Legend_img1.PNG)


### Wrap items

Legend items can also be wrapped one by one as shown in the following screenshot by setting the [`WrapItems`](https://help.syncfusion.com/cr/cref_files/windowsforms/Syncfusion.SfSmithChart.WinForms~Syncfusion.WinForms.SmithChart.ChartLegend~WrapItems.html) property to true. Nearly, 20% of chart area is used for legend. If the items go beyond the view, the vertical scroll bar will be enabled. Based on the dock position, the vertical or horizontal scroll bar will be enabled.

![C:/Users/yogapriya.shanmugam/AppData/Local/Microsoft/Windows/INetCacheContent.Word/LegendWrap.png](Legend_images/Legend_img2.PNG)

