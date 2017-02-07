---
-api-id: T:Windows.UI.Xaml.Media.Animation.Transition
-api-type: winrt class
---

<!-- Class syntax.
public class Transition : Windows.UI.Xaml.DependencyObject, Windows.UI.Xaml.Media.Animation.ITransition
-->

# Windows.UI.Xaml.Media.Animation.Transition

## -description
Represents a visual behavior that occurs for predefined actions or state changes. Specific theme transitions (various [Transition](transition.md) derived classes) can be applied to individual elements using the [UIElement.Transitions](../windows.ui.xaml/uielement_transitions.md) property, or applied for scenario-specific theme transition properties such as [ContentControl.ContentTransitions](../windows.ui.xaml.controls/contentcontrol_contenttransitions.md).

## -remarks
### **Transition** derived classes

[Transition](transition.md) is the parent class for several immediately derived classes that define library theme transitions. Here are some of the notable derived classes:

+ [AddDeleteThemeTransition](adddeletethemetransition.md)
+ [ContentThemeTransition](contentthemetransition.md)
+ [EdgeUIThemeTransition](edgeuithemetransition.md)
+ [EntranceThemeTransition](entrancethemetransition.md)
+ [PaneThemeTransition](panethemetransition.md)
+ [PopupThemeTransition](popupthemetransition.md)
+ [ReorderThemeTransition](reorderthemetransition.md)
+ [RepositionThemeTransition](repositionthemetransition.md)
For each of these classes, you typically define object elements. Most theme transitions don't have additional attributes, so you typically use a basic self-closing object element for example `<PopupThemeTransition />`. These are used to populate a [TransitionCollection](transitioncollection.md) property. Those properties include: 
+ [Border.ChildTransitions](../windows.ui.xaml.controls/border_childtransitions.md)
+ [ContentControl.ContentTransitions](../windows.ui.xaml.controls/contentcontrol_contenttransitions.md)
+ [ContentPresenter.ContentTransitions](../windows.ui.xaml.controls/contentpresenter_contenttransitionsproperty.md)
+ [ItemsControl.ItemContainerTransitions](../windows.ui.xaml.controls/itemscontrol_itemcontainertransitions.md)
+ [ItemsPresenter.FooterTransitions](../windows.ui.xaml.controls/itemspresenter_footertransitions.md)
+ [ItemsPresenter.HeaderTransitions](../windows.ui.xaml.controls/itemspresenter_headertransitions.md)
+ [ListViewBase.FooterTransitions](../windows.ui.xaml.controls/listviewbase_footertransitions.md)
+ [ListViewBase.HeaderTransitions](../windows.ui.xaml.controls/listviewbase_headertransitions.md)
+ [Panel.ChildrenTransitions](../windows.ui.xaml.controls/panel_childrentransitions.md)
+ [Popup.ChildTransitions](../windows.ui.xaml.controls.primitives/popup_childtransitions.md)
+ [SettingsFlyoutTemplateSettings.ContentTransitions](../windows.ui.xaml.controls.primitives/settingsflyouttemplatesettings_contenttransitions.md)
+ [UIElement.Transitions](../windows.ui.xaml/uielement_transitions.md)


Not all transitions make sense for any given property. For example, [PopupThemeTransition](popupthemetransition.md) is really only useful for [Popup.ChildTransitions](../windows.ui.xaml.controls.primitives/popup_childtransitions.md). For more info on how to use the theme transitions, see [Animations overview](http://msdn.microsoft.com/library/0c8dee75-fb7b-4e59-81e3-55f8d65cd982) and topics linked from there, including the design guidelines topics.

> [!IMPORTANT]
> The XAML syntax for all properties that use a [TransitionCollection](transitioncollection.md) value is unusual in that you must declare an explicit [TransitionCollection](transitioncollection.md) object element as the value, and then provide object elements as child elements of [TransitionCollection](transitioncollection.md) for each of the transition animations you want to use. For most other XAML collection properties you could omit the collection object element because it can be implicit, but properties that use [TransitionCollection](transitioncollection.md) don't support the implicit collection usage. For more info on implicit collections and XAML, see [XAML syntax guide](http://msdn.microsoft.com/library/a57fe7b4-9947-4aa0-bc99-5fe4686b611d).

## -examples

## -see-also
[DependencyObject](../windows.ui.xaml/dependencyobject.md), [Animations overview](http://msdn.microsoft.com/library/0c8dee75-fb7b-4e59-81e3-55f8d65cd982), [UIElement.Transitions](../windows.ui.xaml/uielement_transitions.md)