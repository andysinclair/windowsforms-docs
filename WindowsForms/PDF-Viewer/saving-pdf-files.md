---
layout: post
title: Saving PDF Files | PDF Viewer | WinForms | Syncfusion
description: The PDF Viewer supports saving a PDF file loaded in it. It keeps the file up to date with any modifications by allowing you to save the file in the local disk. 
platform: windowsforms
control: PDF Viewer
documentation: ug
---

# Saving PDF Files in PDF Viewer

The Save feature in the [PdfViewerControl](https://help.syncfusion.com/cr/cref_files/windowsforms/Syncfusion.PdfViewer.Windows~Syncfusion.Windows.Forms.PdfViewer.PdfViewerControl.html) helps you to keep the file up to date with any modifications and prevent your work from being lost by allowing you to save the file in the local disk.

![Save option in Toolbar](Save_images/Save.png)

Save can be performed using the following steps.

1.	Open a PDF file in the [PdfViewerControl](https://help.syncfusion.com/cr/cref_files/windowsforms/Syncfusion.PdfViewer.Windows~Syncfusion.Windows.Forms.PdfViewer.PdfViewerControl.html) and do any modifications to the file.
2.	Click the "Save As" icon on the toolbar as shown in the above picture.
3.	In the save dialog box, enter a name, and select "Save".

## Save Notifications

The [PdfViewerControl](https://help.syncfusion.com/cr/cref_files/windowsforms/Syncfusion.PdfViewer.Windows~Syncfusion.Windows.Forms.PdfViewer.PdfViewerControl.html) notifies you at the start and end of the save operation through the [BeginSave](https://help.syncfusion.com/cr/cref_files/windowsforms/Syncfusion.PdfViewer.Windows~Syncfusion.Windows.Forms.PdfViewer.PdfViewerControl~BeginSave_EV.html) and [EndSave](https://help.syncfusion.com/cr/cref_files/windowsforms/Syncfusion.PdfViewer.Windows~Syncfusion.Windows.Forms.PdfViewer.PdfViewerControl~EndSave_EV.html) events respectively.

### Begin Save Event

The [BeginSave](https://help.syncfusion.com/cr/cref_files/windowsforms/Syncfusion.PdfViewer.Windows~Syncfusion.Windows.Forms.PdfViewer.PdfViewerControl~BeginSave_EV.html) event occurs before initiating the save operation of the PDF file. It also allows you to cancel the save operation through the [Cancel](https://help.syncfusion.com/cr/cref_files/windowsforms/Syncfusion.PdfViewer.Windows~Syncfusion.Windows.Forms.PdfViewer.BeginSaveEventArgs~Cancel.html) property of [BeginSaveEventArgs](https://help.syncfusion.com/cr/cref_files/windowsforms/Syncfusion.PdfViewer.Windows~Syncfusion.Windows.Forms.PdfViewer.BeginSaveEventArgs.html). The following code shows how to wire the event in the [PdfViewerControl](https://help.syncfusion.com/cr/cref_files/windowsforms/Syncfusion.PdfViewer.Windows~Syncfusion.Windows.Forms.PdfViewer.PdfViewerControl.html).

{% tabs %}
{% highlight c# %}
using System.Windows.Forms;
using Syncfusion.Windows.Forms.PdfViewer;

namespace SaveEventsDemo
{
    public partial class Form1 : Form
    {
        #region Constructor
        public Form1()
        {
            InitializeComponent();

            //Wire the `BeginSave` event.
            pdfViewerControl1.BeginSave += PdfViewerControl1_BeginSave;

            //Load the PDF file.
            pdfViewerControl1.Load("../../Data/HTTP Succinctly.pdf");
        }
        #endregion

        #region Events
        private void PdfViewerControl1_BeginSave(object sender, BeginSaveEventArgs e)
        {
            //Insert your code here    
        }
        # endregion
    }
}
{% endhighlight %}
{% endtabs %}

### End Save Event

The [EndSave]([EndSave](https://help.syncfusion.com/cr/cref_files/windowsforms/Syncfusion.PdfViewer.Windows~Syncfusion.Windows.Forms.PdfViewer.PdfViewerControl~EndSave_EV.html)) event occurs after the completion of the save operation. The following code shows how to wire the event in the [PdfViewerControl]([PdfViewerControl](https://help.syncfusion.com/cr/cref_files/windowsforms/Syncfusion.PdfViewer.Windows~Syncfusion.Windows.Forms.PdfViewer.PdfViewerControl.html)).

{% tabs %}
{% highlight c# %}
using System.Windows.Forms;
using Syncfusion.Windows.Forms.PdfViewer;

namespace SaveEventsDemo
{
    public partial class Form1 : Form
    {
        #region Constructor
        public Form1()
        {
            InitializeComponent();

            //Wire the `EndSave` event.
            pdfViewerControl1.EndSave += PdfViewerControl1_EndSave;

            //Load the PDF file.
            pdfViewerControl1.Load("../../Data/HTTP Succinctly.pdf");
        }
        #endregion

        #region Events
        private void PdfViewerControl1_EndSave(object sender, EndSaveEventArgs e)
        {
            //Insert your code here
        }
        # endregion
    }
}
{% endhighlight %}
{% endtabs %}

N> The complete sample project of the print events can be downloaded from [GitHub](https://github.com/SyncfusionExamples/WinForms-PDFViewer-Examples/tree/master/Save/SaveEventsDemo).