---
layout: post
title: Theme in winforms form | Syncfusion
description: Learn about theme support in Syncfusion WinForms Form (SfForm) control and more details.
platform: windowsforms
control: SfForm
documentation: ug
---

# Themes

SfForm offers the following six built-in themes for professional representation:

* Office2016Colorful
* Office2016White
* Office2016DarkGray
* Office2016Black
* Office2019Colorful
* HighContrastBlack

Themes can be applied to `SfForm` by following these steps:

* `Load theme assembly`
* `Apply theme`

## Load theme assembly

To set theme to `SfForm`, the following assemblies should be added as reference in any application.

<table>
<tr>
<td>
{{'**Assemblies**'| markdownify }}
</td>
<td>
{{'        **Themes**'| markdownify }}
</td>
</tr>
<tr>
<td>
Syncfusion.Office2016Theme.WinForms       
</td>
<td>
Office2016Colorful<br>
Office2016White<br>
Office2016DarkGray<br>
Office2016Black
</td>
</tr>
<tr>
<td>
Syncfusion.Office2019Theme.WinForms
</td>
<td>
Office2019Colorful
</td>
</tr>
<tr>
<td>
Syncfusion.HighContrastTheme.WinForms
</td>
<td>
HighContrastBlack
</td>
</tr>
</table>

Before applying theme to `SfForm`, required theme assembly should be loaded.

{% tabs %}
{% highlight c# %}
using Syncfusion.WinForms.Controls;

static class Program
{
    /// <summary>
    /// The main entry point for an application.
    /// </summary>
    [STAThread]
    static void Main()
    {
        Syncfusion.Licensing.SyncfusionLicenseProvider.RegisterLicense(DemoCommon.FindLicenseKey());
        SfSkinManager.LoadAssembly(typeof(Syncfusion.WinForms.Themes.Office2016Theme).Assembly);
        SfSkinManager.LoadAssembly(typeof(Syncfusion.WinForms.Themes.Office2019Theme).Assembly);
        SfSkinManager.LoadAssembly(typeof(Syncfusion.HighContrastTheme.WinForms.HighContrastTheme).Assembly);
        Application.EnableVisualStyles();
        Application.SetCompatibleTextRenderingDefault(false);
        Application.Run(new Form1());
    }
}
{% endhighlight %}
{% highlight vb %}
Imports Syncfusion.WinForms.Controls

Friend NotInheritable Class Program
	''' <summary>
	''' The main entry point for the application.
	''' </summary>
	Private Sub New()
	End Sub
	<STAThread>
	Shared Sub Main()
		Syncfusion.Licensing.SyncfusionLicenseProvider.RegisterLicense(DemoCommon.FindLicenseKey())
		SfSkinManager.LoadAssembly(GetType(Syncfusion.WinForms.Themes.Office2016Theme).Assembly)
		SfSkinManager.LoadAssembly(GetType(Syncfusion.WinForms.Themes.Office2019Theme).Assembly)
		SfSkinManager.LoadAssembly(GetType(Syncfusion.HighContrastTheme.WinForms.HighContrastTheme).Assembly)
		Application.EnableVisualStyles()
		Application.SetCompatibleTextRenderingDefault(False)
		Application.Run(New Form1())
	End Sub
End Class
{% endhighlight %}
{% endtabs %}

## Apply theme

The appearance of `SfForm` can be changed using [ThemeName](https://help.syncfusion.com/cr/windowsforms/Syncfusion.Shared.Base~Syncfusion.WinForms.Controls.SfForm~ThemeName.html) of `SfForm`.

### Office2016Colorful

This option helps to set the Office2016Colorful theme.

{% tabs %}
{% highlight c# %}
 sfForm.ThemeName = "Office2016Colorful";
{% endhighlight %}
{% highlight vb %}
 sfForm.ThemeName = "Office2016Colorful"
{% endhighlight %}
{% endtabs %}

![SfForm](Themes_images/Themes_img1.png)

### Office2016White

This option helps to set the Office2016White theme.

{% tabs %}
{% highlight c# %}
 sfForm.ThemeName = "Office2016White";
{% endhighlight %}
{% highlight vb %}
 sfForm.ThemeName = "Office2016White"
{% endhighlight %}
{% endtabs %}

![SfForm](Themes_images/Themes_img2.png)

### Office2016DarkGray

This option helps to set the Office2016DarkGray theme.

{% tabs %}
{% highlight c# %}
 sfForm.ThemeName = "Office2016DarkGray";
{% endhighlight %}
{% highlight vb %}
 sfForm.ThemeName = "Office2016DarkGray"
{% endhighlight %}
{% endtabs %}

![SfForm](Themes_images/Themes_img3.png)

### Office2016Black

This option helps to set the Office2016Black theme.

{% tabs %}
{% highlight c# %}
 sfForm.ThemeName = "Office2016Black";
{% endhighlight %}
{% highlight vb %}
 sfForm.ThemeName = "Office2016Black"
{% endhighlight %}
{% endtabs %}

![SfForm](Themes_images/Themes_img4.png)

### Office2019Colorful

This option helps to set the Office2019Colorful theme.

{% tabs %}
{% highlight c# %}
 sfForm.ThemeName = "Office2019Colorful";
{% endhighlight %}
{% highlight vb %}
 sfForm.ThemeName = "Office2019Colorful"
{% endhighlight %}
{% endtabs %}

![SfForm](Themes_images/Themes_img5.png)

### HighContrastBlack

This option helps to set the HighContrastBlack theme.

{% tabs %}
{% highlight c# %}
 sfForm.ThemeName = "HighContrastBlack";
{% endhighlight %}
{% highlight vb %}
 sfForm.ThemeName = "HighContrastBlack"
{% endhighlight %}
{% endtabs %}

![SfForm](Themes_images/Themes_img6.png)