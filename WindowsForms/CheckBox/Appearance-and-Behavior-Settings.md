---
layout: post
title: Appearance-and-Behavior-Settings | WindowsForms | Syncfusion
description: appearance and behavior settings
platform: WindowsForms
control: EditorsPackage
documentation: ug
---

# Appearance and Behavior Settings

This section discusses the appearance and behavior settings of the CheckBoxAdv control.

## Appearance Settings

### DrawFocusRectangle

The focus rectangle can be hidden or made visible using the below given property.

<table>
<tr>
<th>
CheckBoxAdv Property</th><th>
Description</th></tr>
<tr>
<td>
DrawFocusRectangle</td><td>
Determines if the focus rectangle is visible when it gets the focus. The default value is set to 'True'.</td></tr>
</table>

{% tabs %}
{% highlight c# %}

this.checkBoxAdv1.DrawFocusRectangle = true;

{% endhighlight %}

{% highlight vb %}

Me.checkBoxAdv1.DrawFocusRectangle = True

{% endhighlight %}
{% endtabs %}

![Windows forms CheckBoxAdv drawFocusRectangle is enabled or diabled](Overview_images/CheckBoxAdv_focus.jpeg)

## Behavior Settings

The behavior settings of the CheckBoxAdv can be customized using the properties given below.


<table>
<tr>
<th>
CheckBoxAdv Properties</th><th>
Description</th></tr>
<tr>
<td>
AutoHeight</td><td>
Determines if the CheckBoxAdv will automatically calculate its height.</td></tr>
<tr>
<td>
ReadOnlyMode</td><td>
Specifies the Read Only Mode of the CheckBoxAdv.</td></tr>
<tr>
<td>
Tristate</td><td>
Specifies whether the indeterminate state can be accessed through clicking.</td></tr>
</table>

{% tabs %}
{% highlight c# %}

this.checkBoxAdv1.AutoHeight = true;
this.checkBoxAdv1.ReadOnlyMode = true;
this.checkBoxAdv1.Tristate= false;

{% endhighlight %}

{% highlight vb %}

Me.checkBoxAdv1.AutoHeight = True
Me.checkBoxAdv1.ReadOnlyMode = True
Me.checkBoxAdv1.Tristate= False

{% endhighlight %}
{% endtabs %}
