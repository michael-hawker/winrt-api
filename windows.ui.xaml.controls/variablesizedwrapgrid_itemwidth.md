---
-api-id: P:Windows.UI.Xaml.Controls.VariableSizedWrapGrid.ItemWidth
-api-type: winrt property
---

<!-- Property syntax
public double ItemWidth { get;  set; }
-->

# Windows.UI.Xaml.Controls.VariableSizedWrapGrid.ItemWidth

## -description
Gets or sets the width of the layout area for each item that is contained in a [VariableSizedWrapGrid](variablesizedwrapgrid.md).

## -xaml-syntax
```xaml
<VariableSizedWrapGrid ItemWidth="double" />
-or-
<VariableSizedWrapGrid ItemWidth="Auto" />
```


## -property-value
The width of the layout area for each item that is contained in a [VariableSizedWrapGrid](variablesizedwrapgrid.md). The default is [Double.NaN](https://msdn.microsoft.com/library/system.double.nan.aspx), which results in the "Auto" layout behavior.

## -remarks
### "Auto" layout and Double.NaN

The default value of [ItemHeight](variablesizedwrapgrid_itemheight.md) and [ItemWidth](variablesizedwrapgrid_itemwidth.md) is not 0, it is [Double.NaN](https://msdn.microsoft.com/library/system.double.nan.aspx). [ItemHeight](variablesizedwrapgrid_itemheight.md) and [ItemWidth](variablesizedwrapgrid_itemwidth.md) support the ability to be an unset "Auto" value. Because [ItemHeight](variablesizedwrapgrid_itemheight.md) and [ItemWidth](variablesizedwrapgrid_itemwidth.md) are **Double** values, [Double.NaN](https://msdn.microsoft.com/library/system.double.nan.aspx) is used as a special value to represent this "Auto" behavior. The layout system interprets the "Auto" value to generally mean that the object should be sized to the available size in layout, instead of to a specific pixel value. If you want the "Auto" behavior for an object when it is used in layout, leave [ItemHeight](variablesizedwrapgrid_itemheight.md) and [ItemWidth](variablesizedwrapgrid_itemwidth.md) unset at their [Double.NaN](https://msdn.microsoft.com/library/system.double.nan.aspx) default value. If you have previously set values and want to reenable the "Auto" behavior with run-time code, set to [Double.NaN](https://msdn.microsoft.com/library/system.double.nan.aspx). In XAML such as templates, you can set attribute values using the string "Auto". 
<!--Setting Auto in XAML is a special behavior of the XAML parser, not a TypeConverter behavior.-->


> [!NOTE]
> Visual C++ component extensions (C++/CX) doesn't have a constant for **NaN**, it uses a value, which appears as "-1.#IND" followed by zeros.

## -examples

## -see-also
[ItemHeight](variablesizedwrapgrid_itemheight.md)