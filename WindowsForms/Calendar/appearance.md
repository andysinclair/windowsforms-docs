---
layout: post
title: Appearance of SfCalendar | WindowsForms | Syncfusion
description: This section explains how to customize the appearance of header, footer, and cells in the calendar and various styles available in SfCalendar.
platform: WindowsForms
control: SfCalendar
documentation: ug
---

# Appearance

This section explains how to customize the appearance of header, footer, and cells in the calendar by using [style](https://help.syncfusion.com/cr/windowsforms/Syncfusion.SfInput.WinForms~Syncfusion.WinForms.Input.SfCalendar~Style.html) properties.

## Customize header appearance

The BackColor and ForeColor of each part in the calendar header can be customized. The height of the calendar header can be customized by using the [HeaderHeight](https://help.syncfusion.com/cr/windowsforms/Syncfusion.SfInput.WinForms~Syncfusion.WinForms.Input.SfCalendar~HeaderHeight.html) property, and the width of header can be updated automatically from the calendar width.

### Customize header text

The header text in the calendar control displays the month and year of the selected date. The calendar header color can be customized by using the following style properties:

* BackColor: Changes the background color of header in the calendar.
* ForeColor: Changes the foreground color of the text, which displays month and year in the calendar header.
* HoverForeColor: Changes the foreground color of the header text on mouse hover.
* Font: Changes the font that is used to draw the header text in the calendar.

### Customize day names

The calendar header contains day names of week for the month view. Day names of the calendar header can be customized by using the following properties:

* DayNamesBackColor: Changes the background color of day names in the calendar header.
* DayNamesForeColor: Changes the foreground color of day names in the calendar header.
* DayNamesFont: Changes the font that is used to draw the day names text in the calendar.

The following code example illustrates how to customize appearances of the calendar header:

{% tabs %}

{% highlight C# %}

// Header customizations

// Setting header BackColor

this.sfCalendar.Style.Header.BackColor = Color.Red;

// Setting header ForeColor

this.sfCalendar.Style.Header.ForeColor = Color.Yellow;

// Setting header DayNames BackColor

this.sfCalendar.Style.Header.DayNamesBackColor = Color.Green;

// Setting header DayNames ForeColor

this.sfCalendar.Style.Header.DayNamesForeColor = Color.WhiteSmoke;

// Setting header DayNames Font

this.sfCalendar.Style.Header.DayNamesFont = new System.Drawing.Font("Calibri", 11.25F, System.Drawing.FontStyle.Regular);

{% endhighlight  %}

{% highlight VB %}

' Header customizations

' Setting header BackColor

Me.sfCalendar.Style.Header.BackColor = Color.LightGray

' Setting header ForeColor

Me.sfCalendar.Style.Header.ForeColor = Color.Blue

' Setting header DayNames BackColor

Me.sfCalendar.Style.Header.DayNamesBackColor = Color.LightSeaGreen

' Setting header DayNames ForeColor

Me.sfCalendar.Style.Header.DayNamesForeColor = Color.AliceBlue

' Setting header DayNames Font

Me.sfCalendar.Style.Header.DayNamesFont = New System.Drawing.Font("Calibri", 11.25!, System.Drawing.FontStyle.Regular)

{% endhighlight  %}

{% endtabs %} 

![SfCalendar header customization](appearance-images/headercustomizations.png)

## Customize navigation buttons

Navigation buttons in the calendar header can be customized by changing the up and down icons. Icons used for navigation buttons can be changed by `UpArrowImage` and `DownArrowImage` properties of the SfCalendar. The color used to draw the default icons for up and down navigation buttons can be customized by the following properties:

* NavigationButtonForeColor: Changes the foreground color of up and down navigation buttons.
* NavigationButtonHoverForeColor: Changes the foreground color of up and down navigation buttons on mouse hover.
* NavigationButtonDisabledForeColor: Changes the foreground color of up and down navigation buttons in disabled state.

The following code example illustrates the same:

{% tabs %}

{% highlight C# %}

// set the Navigation Button ForeColor
            
this.sfCalendar.Style.Header.NavigationButtonForeColor = Color.HotPink;

// set the Navigation Button Hover ForeColor

this.sfCalendar.Style.Header.NavigationButtonHoverForeColor = Color.Indigo;

// set the Navigation Button disabled ForeColor
            
this.sfCalendar.Style.Header.NavigationButtonDisabledForeColor = Color.LightGray;

{% endhighlight  %}

{% highlight VB %}

' set the Navigation Button ForeColor

Me.sfCalendar.Style.Header.NavigationButtonForeColor = Color.HotPink

' set the Navigation Button Hover ForeColor

Me.sfCalendar.Style.Header.NavigationButtonHoverForeColor = Color.Indigo

' set the Navigation Button disabled ForeColor

Me.sfCalendar.Style.Header.NavigationButtonDisabledForeColor = Color.LightGray

The visibility and alignment of navigation buttons can also be customized.

{% endhighlight  %}

{% endtabs %} 

![Navigation button color customization](appearance-images/navigationcolor.png)

### Visibility of navigation buttons

Navigation buttons are used to move between views in the `SfCalendar`. The visibility of navigation buttons can be customized by the [ShowNavigationButton](https://help.syncfusion.com/cr/windowsforms/Syncfusion.SfInput.WinForms~Syncfusion.WinForms.Input.SfCalendar~ShowNavigationButton.html) property. The following code example illustrates the same:

{% tabs %}

{% highlight C# %}

// Indicating whether show the navigation buttons which used to move between views. 

this.sfCalendar.ShowNavigationButton = false;

{% endhighlight  %}

{% highlight VB %}

' Indicating whether  show the navigation buttons which used to move between views. 

Me.sfCalendar.ShowNavigationButton = false

{% endhighlight  %}

{% endtabs %}

![Hide the navigation buttons](appearance-images/navigationbuttons.png)

### Navigation buttons alignment

Navigation buttons can be aligned in different sides relative to the calendar header. The alignment of navigation buttons can be customized by the [NavigationButtonAlignment](https://help.syncfusion.com/cr/windowsforms/Syncfusion.SfInput.WinForms~Syncfusion.WinForms.Input.SfCalendar~NavigationButtonAlignment.html). The following code example illustrates the same:

{% tabs %}

{% highlight C# %}

// Indicating how the navigation buttons should align relative to the Calendar Header. Setting Left alignment. 

this.sfCalendar.NavigationButtonAlignment = Syncfusion.WinForms.Input.Enums.NavigationButtonAlignment.Left;

{% endhighlight  %}

{% highlight VB %}

' Indicating how the navigation buttons should align relative to the Calendar Header. Setting Left alignment. 

Me.sfCalendar.NavigationButtonAlignment = Syncfusion.WinForms.Input.Enums.NavigationButtonAlignment.Left

{% endhighlight  %}

{% endtabs %}

![Navigation buttons alignment](appearance-images/navbuttonalignleft.png)

{% tabs %}

{% highlight C# %}

// Indicating how the navigation buttons should align relative to the Calendar Header. Setting Both alignment. 

this.sfCalendar.NavigationButtonAlignment = Syncfusion.WinForms.Input.Enums.NavigationButtonAlignment.Both;

{% endhighlight  %}

{% highlight VB %}

' Indicating how the navigation buttons should align relative to the Calendar Header. Setting Both alignment. 

Me.sfCalendar.NavigationButtonAlignment = Syncfusion.WinForms.Input.Enums.NavigationButtonAlignment.Both

{% endhighlight  %}

{% endtabs %}

![Both navigation buttons alignment](appearance-images/navbuttonalignboth.png)

## Customize footer appearance

The BackColor and ForeColor of each part in the calendar footer can be customized. The height of the calendar footer can be customized by using the [FooterHeight](https://help.syncfusion.com/cr/windowsforms/Syncfusion.SfInput.WinForms~Syncfusion.WinForms.Input.SfCalendar~FooterHeight.html) property, and the width of the footer can be updated automatically from the calendar width. The calendar control footer color can be customized by the following style properties:

* BackColor: Changes the background color of footer in the calendar.
* ForeColor: Changes the foreground color of footer in the calendar.
* HoverBackColor: Changes the background color of footer on mouse hover.
* HoverForeColor: Changes the foreground color of footer text on mouse hover.

The following code example illustrates how to change the background and foreground of the calendar footer:

{% tabs %}

{% highlight C# %}

// Footer customizations

// Setting Footer BackColor

this.sfCalendar.Style.Footer.BackColor = Color.LightGreen;

// Setting Footer ForeColor

this.sfCalendar.Style.Footer.ForeColor = Color.Green;

// Setting Footer HoverBackColor

this.sfCalendar.Style.Footer.HoverBackColor = Color.Yellow;

// Setting Footer HoverForeColor

this.sfCalendar.Style.Footer.HoverForeColor = Color.SpringGreen;

{% endhighlight  %}

{% highlight VB %}

' Footer customizations

' Setting Footer BackColor

Me.sfCalendar.Style.Footer.BackColor = Color.LightGreen

' Setting Footer ForeColor

Me.sfCalendar.Style.Footer.ForeColor = Color.Green

' Setting Footer HoverBackColor

Me.sfCalendar.Style.Footer.HoverBackColor = Color.Yellow

' Setting Footer HoverForeColor

Me.sfCalendar.Style.Footer.HoverForeColor = Color.SpringGreen

{% endhighlight  %}

{% endtabs %} 

![Footer customization](appearance-images/footercustomizations.png)

## Customize cell appearance

BackColor, ForeColor, and BorderColor of each date cells in the calendar can be customized. Date cells in the calendar control can be customized by the following style properties:

* CellBackColor: Changes the background color of date cells in the calendar.
* CellForeColor: Changes the foreground color of date cells in the calendar.
* CellHoverBorderColor: Changes the border color of date cells in the calendar.
* CellFont: Changes the font that is used to draw the date text of cell in the calendar.

### Customize trailing date appearance

Calendar control trailing (next or previous month) cells can be customized by the following properties:

* TrailingCellBackColor: Changes the background color of the previous and following month cells that are shown in the current view of the calendar.
* TrailingCellForeColor: Changes the foreground color of the previous and following month cells that are shown in the current view of the calendar.
* TrailingCellFont: Changes the font that is used to draw the date text for the previous and following month cells that are shown in the current view of the calendar.

### Customize selected date appearance

The BackColor and ForeColor of the selected date cell in the calendar can customized. The following code illustrates how to customize the selected date cell appearance:

* SelectedCellBackColor: Changes the background color of the selected date cell in the calendar.
* SelectedCellForeColor: Changes the foreground color of the selected date cell in the calendar.
* SelectedCellBorderColor: Changes the border color of the selected date cell in the calendar.
* SelectedCellHoverBorderColor: Changes the border color of the selected date cell on mouse hover.
* SelectedCellFont: Changes the font that is used to draw the date text of the selected date cell in the calendar.

The following code example illustrates the customization of calendar cells:

{% tabs %}

{% highlight C# %}

// Setting CellBackColor

this.sfCalendar.Style.Cell.CellBackColor = Color.LightBlue;

// Setting CellForeColor

this.sfCalendar.Style.Cell.CellForeColor = Color.Red;

// Setting CellHoverBorderColor

this.sfCalendar.Style.Cell.CellHoverBorderColor = Color.LightCyan;

// Setting SelectedCellBackColor

this.sfCalendar.Style.Cell.SelectedCellBackColor = Color.Blue;

// Setting SelectedCellForeColor

this.sfCalendar.Style.Cell.SelectedCellForeColor = Color.White;

// Setting SelectedCellBorderColor

this.sfCalendar.Style.Cell.SelectedCellBorderColor = Color.Tomato;

// Setting SelectedCellHoverBorderColor

this.sfCalendar.Style.Cell.SelectedCellHoverBorderColor = Color.Yellow;

// Setting TrailingCellBackColor

this.sfCalendar.Style.Cell.TrailingCellBackColor = Color.LightGray;

// Setting TrailingCellForeColor

this.sfCalendar.Style.Cell.TrailingCellForeColor = Color.Black;

// Setting TrailingCellFont

this.sfCalendar.Style.Cell.TrailingCellFont = new System.Drawing.Font("Calibri", 11.25F, System.Drawing.FontStyle.Bold);

// Setting CellFont

this.sfCalendar.Style.Cell.CellFont = new System.Drawing.Font("Calibri", 11.25F, System.Drawing.FontStyle.Bold);

// Setting selected CellFont

this.sfCalendar.Style.Cell.SelectedCellFont = new System.Drawing.Font("Calibri", 11.25F, System.Drawing.FontStyle.Regular); 

{% endhighlight  %}

{% highlight VB %}

' Setting CellBackColor

Me.sfCalendar.Style.Cell.CellBackColor = Color.LightBlue

' Setting CellForeColor

Me.sfCalendar.Style.Cell.CellForeColor = Color.Red

' Setting CellHoverBorderColor

Me.sfCalendar.Style.Cell.CellHoverBorderColor = Color.LightCyan

' Setting SelectedCellBackColor

Me.sfCalendar.Style.Cell.SelectedCellBackColor = Color.Blue

' Setting SelectedCellForeColor

Me.sfCalendar.Style.Cell.SelectedCellForeColor = Color.White

' Setting SelectedCellBorderColor

Me.sfCalendar.Style.Cell.SelectedCellBorderColor = Color.Tomato

' Setting SelectedCellHoverBorderColor

Me.sfCalendar.Style.Cell.SelectedCellHoverBorderColor = Color.Yellow

' Setting TrailingCellBackColor

Me.sfCalendar.Style.Cell.TrailingCellBackColor = Color.LightGray

' Setting TrailingCellForeColor

Me.sfCalendar.Style.Cell.TrailingCellForeColor = Color.Black

' Setting TrailingCellFont

Me.sfCalendar.Style.Cell.TrailingCellFont = New System.Drawing.Font("Calibri", 11.25!, System.Drawing.FontStyle.Bold)

' Setting CellFont

Me.sfCalendar.Style.Cell.CellFont = New System.Drawing.Font("Calibri", 11.25!, System.Drawing.FontStyle.Bold)

' Setting selected CellFont

Me.sfCalendar.Style.Cell.SelectedCellFont = New System.Drawing.Font("Calibri", 11.25!, System.Drawing.FontStyle.Regular)

{% endhighlight  %}

{% endtabs %} 

![Cell appearance](appearance-images/cellcustomization.png)

## Themes

SfCalendar offers four built in themes for professional representation as follows.

* Office2016Colorful
* Office2016White
* Office2016DarkGray
* Office2016Black

Theme can be applied to SfCalendar by following the below steps:

1. [Load theme assembly](#load-theme-assembly)
2. [Apply theme](#apply-theme)

### Load theme assembly

**Syncfusion.Office2016Theme.WinForms** assembly should be added as reference to set theme for SfCalendar in any application:

Before apply theme to SfCalendar, required theme assembly should be loaded as follows. 

{% tabs %}

{% highlight C# %}

using Syncfusion.WinForms.Core.Events;

         static class Program
    {
        /// <summary>
        /// The main entry point for the application.
        /// </summary>
        
        static void Main()
        {
            SfSkinManager.LoadAssembly(typeof(Office2016Theme).Assembly);
            Application.EnableVisualStyles();
            Application.SetCompatibleTextRenderingDefault(false);
            Application.Run(new Form1());
        }
    }

{% endhighlight  %}

{% highlight VB %}

Imports Syncfusion.WinForms.Core.Events

 Friend Module Program
        ''' <summary>
        ''' The main entry point for the application.
        ''' </summary>
        <STAThread>
        Sub Main()
            SfSkinManager.LoadAssembly(GetType(Office2016Theme).Assembly)
            Application.EnableVisualStyles()
            Application.SetCompatibleTextRenderingDefault(False)
            Application.Run(New Form1())
        End Sub
    End Module

{% endhighlight  %}

{% endtabs %}

### Apply theme

Appearance of SfCalendar can be changed by [ThemeName](https://help.syncfusion.com/cr/windowsforms/Syncfusion.SfInput.WinForms~Syncfusion.WinForms.Input.SfCalendar~ThemeName.html) of SfCalendar.

#### Office2016Colorful

This option helps to set the Office2016Colorful Theme.

{% tabs %}

{% highlight C# %}

// Office2016Colorful

 this.sfCalendar.ThemeName = "Office2016Colorful";

{% endhighlight  %}

{% highlight VB %}

' Office2016Colorful 

Me.sfCalendar.ThemeName = "Office2016Colorful"

{% endhighlight  %}

{% endtabs %}

![SfCalendar Office2016Colorful theme](appearance-images/Office2016Colorful.png)

#### Office2016White

This option helps to set the Office2016White Theme.

{% tabs %}

{% highlight C# %}

// Office2016White

 this.sfCalendar.ThemeName = "Office2016White";

{% endhighlight  %}

{% highlight VB %}

' Office2016White 

Me.sfCalendar.ThemeName = "Office2016White"

{% endhighlight  %}

{% endtabs %}

![SfCalendar Office2016White theme](appearance-images/Office2016White.png)

#### Office2016DarkGray

This option helps to set the Office2016DarkGray Theme.

{% tabs %}

{% highlight C# %}

// Office2016DarkGray

 this.sfCalendar.ThemeName = "Office2016DarkGray";

{% endhighlight  %}

{% highlight VB %}

' Office2016DarkGray 

Me.sfCalendar.ThemeName = "Office2016DarkGray"

{% endhighlight  %}

{% endtabs %}

![SfCalendar Office2016DarkGray theme](appearance-images/Office2016DarkGray.png)

#### Office2016Black

This option helps to set the Office2016Black Theme.

{% tabs %}

{% highlight C# %}

// Office2016Black

 this.sfCalendar.ThemeName = "Office2016Black";

{% endhighlight  %}

{% highlight VB %}

' Office2016Black 

Me.sfCalendar.ThemeName = "Office2016Black"

{% endhighlight  %}

{% endtabs %}

![SfCalendar Office2016Black theme](appearance-images/Office2016Black.png)

## Hide trailing dates   

The `SfCalendar` allows you to hide the days of next month and previous month in the calendar to enhance the appearance of the calendar. This can be achieved by disabling the [TrailingDatesVisible](https://help.syncfusion.com/cr/windowsforms/Syncfusion.SfInput.WinForms~Syncfusion.WinForms.Input.SfCalendar~TrailingDatesVisible.html) property. The following code example illustrates how to hide trailing dates in the calendar:

{% tabs %}

{% highlight C# %}

// Setting the Next and Previous Months Dates invisible

this.SfCalendar1.TrailingDatesVisible = false;

{% endhighlight  %}

{% highlight VB %}

' Setting the Next and Previous Months Dates invisible

this.SfCalendar1.TrailingDatesVisible = False

{% endhighlight  %}

{% endtabs %}

![Hide trailing dates](appearance-images/inactivedaysfalse.png)

## Abbreviating day names

By default, the day names are displayed in an abbreviated form in the calendar control. They can also be displayed in an expanded form by setting the [ShowAbbreviatedDayNames](https://help.syncfusion.com/cr/windowsforms/Syncfusion.SfInput.WinForms~Syncfusion.WinForms.Input.SfCalendar~ShowAbbreviatedDayNames.html) property to false. This indicates whether the name of day is abbreviated or expanded. The following code example illustrates how to display the day names in an expanded form:

{% tabs %}

{% highlight C# %}

// Setting the Show Abbreviated Day Names

this.sfCalendar.ShowAbbreviatedDayNames = false;

{% endhighlight  %}

{% highlight VB %}

' Setting the Show Abbreviated Day Names

Me.sfCalendar.ShowAbbreviatedDayNames = false

{% endhighlight  %}

{% endtabs %}

![Abbreviating day names](appearance-images/abbreviateddaynames.png)

## Right-to-left

`SfCalendar` control elements can be aligned in right-to-left layout. The `SfCalendar` control is laid out from the right to left when the `RightToLeft` value is set to `Yes`. The following code example illustrates the same:

{% tabs %}

{% highlight C# %}

//Enable the Right to Left 

this.sfCalendar.RightToLeft = RightToLeft.Yes;

{% endhighlight  %}

{% highlight VB %}

'Enable the Right to Left 

Me.sfCalendar.RightToLeft = RightToLeft.Yes

{% endhighlight  %}

{% endtabs %}

![Right to left support](appearance-images/righttoleft.png)

## Highlight today cell 

The today cell will be highlighted even the selected date differs from today in the `SfCalendar`. The highlight of today cell can be changed by the [HighlightTodayCell](https://help.syncfusion.com/cr/windowsforms/Syncfusion.SfInput.WinForms~Syncfusion.WinForms.Input.SfCalendar~HighlightTodayCell.html) property. The today date cell can also be customized by using the following style properties. The following code snippets illustrates the same:

{% tabs %}

{% highlight C# %}

// Indicating whether Today cell highlighted even selected date is different than today

this.sfCalendar.HighlightTodayCell = true;

{% endhighlight  %}

{% highlight VB %}

' Indicating whether Today cell highlighted even selected date is different than Today

Me.sfCalendar.HighlightTodayCell = true

{% endhighlight  %}

{% endtabs %}

![Highlight today cell](appearance-images/todaycell.png)

### Customize today cell appearance

The BackColor, ForeColor, and BorderColor of the today cell in the calendar can be customized. The today cell in the calendar control can be customized by using the following style properties:

* TodayBackColor: Changes the background color of today cell in the calendar.
* TodayForeColor: Changes the foreground color of today cell in the calendar.
* TodayFont: Changes the font that is used to draw the date text of today cell in the calendar.
* TodayHoverBorderColor: Changes the border color of today cell on mouse hover.

## Change visibility of the footer

The visibility of the calendar footer can be customized by using the [ShowFooter](https://help.syncfusion.com/cr/windowsforms/Syncfusion.SfInput.WinForms~Syncfusion.WinForms.Input.SfCalendar~ShowFooter.html) property which contains today and none buttons. The visibility of today and none buttons can be represented separately by [ShowToday](https://help.syncfusion.com/cr/windowsforms/Syncfusion.SfInput.WinForms~Syncfusion.WinForms.Input.SfCalendar~ShowToday.html) and [ShowNone](https://help.syncfusion.com/cr/windowsforms/Syncfusion.SfInput.WinForms~Syncfusion.WinForms.Input.SfCalendar~ShowNone.html) properties respectively. The following code example illustrates the same:

{% tabs %}

{% highlight C# %}

// Indicating the visibility of none button in footer 

this.sfCalendar.ShowFooter = true;

this.sfCalendar.ShowNone = false;

{% endhighlight  %}

{% highlight VB %}

' Indicating the visibility of none button in footer 

Me.sfCalendar.ShowFooter = true

Me.sfCalendar.ShowNone = false

{% endhighlight  %}

{% endtabs %}

![Show today button](appearance-images/showtoday.png)

{% tabs %}

{% highlight C# %}

// Indicating the visibility of today button in footer 

this.sfCalendar.ShowFooter = true;

this.sfCalendar.ShowToday = false;

{% endhighlight  %}

{% highlight VB %}

' Indicating the visibility of today button in footer 

Me.sfCalendar.ShowFooter = true

Me.sfCalendar.ShowToday = false

{% endhighlight  %}

{% endtabs %}

![show none button](appearance-images/shownone.png)

## Customize splitter appearance

The visibility of splitters in the calendar control can be customized by setting the [ShowHorizontalSplitter](https://help.syncfusion.com/cr/windowsforms/Syncfusion.SfInput.WinForms~Syncfusion.WinForms.Input.SfCalendar~ShowHorizontalSplitter.html) and [ShowVerticalSplitter](https://help.syncfusion.com/cr/windowsforms/Syncfusion.SfInput.WinForms~Syncfusion.WinForms.Input.SfCalendar~ShowVerticalSplitter.html) properties. The splitters color for horizontal and vertical splitters can be customized by the [HorizontalSplitterColor](https://help.syncfusion.com/cr/windowsforms/Syncfusion.SfInput.WinForms~Syncfusion.WinForms.Input.Styles.CalendarVisualStyle~HorizontalSplitterColor.html) and [VerticalSplitterColor](https://help.syncfusion.com/cr/windowsforms/Syncfusion.SfInput.WinForms~Syncfusion.WinForms.Input.Styles.CalendarVisualStyle~VerticalSplitterColor.html) respectively. The following code example illustrates the same:

{% tabs %}

{% highlight C# %}

// Enable Horizontal splitter

 this.sfCalendar.ShowHorizontalSplitter = true;

// Enable Vertical splitter

this.sfCalendar.ShowVerticalSplitter = true;

//  color used draw the Horizontal splitter in cell view

this.sfCalendar.Style.HorizontalSplitterColor = Color.Red;

// color used draw the vertical splitter in cell view

this.sfCalendar.Style.VerticalSplitterColor = Color.Green;

{% endhighlight  %}

{% highlight VB %}

' Enable Horizontal splitter

Me.sfCalendar.ShowHorizontalSplitter = true

' Enable Vertical splitter

Me.sfCalendar.ShowVerticalSplitter = true

'  color used draw the Horizontal splitter in cell view

Me.sfCalendar.Style.HorizontalSplitterColor = Color.Red

' color used draw the vertical splitter in cell view

Me.sfCalendar.Style.VerticalSplitterColor = Color.Green

{% endhighlight  %}

{% endtabs %}

![Customize splitter appearance](appearance-images/splittercolor.png)