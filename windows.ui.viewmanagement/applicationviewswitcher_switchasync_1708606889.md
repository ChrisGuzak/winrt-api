---
-api-id: M:Windows.UI.ViewManagement.ApplicationViewSwitcher.SwitchAsync(System.Int32,System.Int32)
-api-type: winrt method
---

<!-- Method syntax
public Windows.Foundation.IAsyncAction SwitchAsync(System.Int32 toViewId, System.Int32 fromViewId)
-->

# Windows.UI.ViewManagement.ApplicationViewSwitcher.SwitchAsync

## -description

Visually switches the calling window (app view) to a specified window.

## -parameters

### -param toViewId

The ID of the window under preparation for display.

### -param fromViewId

The ID of the calling, currently displayed window.

## -returns

The asynchronous results of the operation. Use this to determine when the async call is complete.

## -remarks

Unlike [SwitchAsync(System.Int32 viewId)](applicationviewswitcher_switchasync_1398322393.md), this method specifies *fromViewId* and frees the caller from executing the call on the Application Single-Threaded Apartment (ASTA) thread of the "from" view. By explicitly passing the same view ID as that inferred through the SwitchAsync(Int32) call, the result of the calls is identical.

## -examples

## -see-also

[SwitchAsync(Int32)](applicationviewswitcher_switchasync_1398322393.md), [SwitchAsync(Int32, Int32, ApplicationViewSwitchingOptions)](applicationviewswitcher_switchasync_1967756911.md)