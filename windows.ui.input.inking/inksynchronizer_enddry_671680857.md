---
-api-id: M:Windows.UI.Input.Inking.InkSynchronizer.EndDry
-api-type: winrt method
---

<!-- Method syntax
public void EndDry()
-->

# Windows.UI.Input.Inking.InkSynchronizer.EndDry

## -description
Finalizes a custom "dry" of ink input to the Direct2D device context of your app, instead of the default [InkCanvas](../windows.ui.xaml.controls/inkcanvas.md) control, and notifies the system that "wet" ink can be removed. This requires an [IInkD2DRenderer](XREF:TODO:input_ink.iinkd2drenderer) object to manage the ink input (see the [Complex ink sample](http://go.microsoft.com/fwlink/p/?LinkID=620314)).

By default, ink input is processed on a low-latency background thread and rendered "wet" as it is drawn. When the stroke is completed (pen or finger lifted, or mouse button released), the stroke is processed on the UI thread and rendered "dry" to the [InkCanvas](../windows.ui.xaml.controls/inkcanvas.md) layer (above the application content and replacing the wet ink).

By calling [ActivateCustomDrying](inkpresenter_activatecustomdrying.md) (before the [InkCanvas](../windows.ui.xaml.controls/inkcanvas.md) is loaded), an app creates an [InkSynchronizer](inksynchronizer.md) object to customize how an ink stroke is rendered dry to a [SurfaceImageSource](../windows.ui.xaml.media.imaging/surfaceimagesource.md) or [VirtualSurfaceImageSource](../windows.ui.xaml.media.imaging/virtualsurfaceimagesource.md). For example, an ink stroke could be rasterized and integrated into application content instead of as a separate [InkCanvas](../windows.ui.xaml.controls/inkcanvas.md) layer.

## -remarks

## -examples

## -see-also
[Pen and stylus interactions](http://msdn.microsoft.com/library/3da4f2d2-5405-42a1-9ed9-3a87bcd84c43), [Ink sample](http://go.microsoft.com/fwlink/p/?LinkID=620308), [Simple ink sample](http://go.microsoft.com/fwlink/p/?LinkID=620312), [Complex ink sample](http://go.microsoft.com/fwlink/p/?LinkID=620314)