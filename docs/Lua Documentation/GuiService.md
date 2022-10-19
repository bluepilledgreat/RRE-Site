# GuiService

## Properties

TODO

## Methods

AddCenterDialog(Instance dialog, Enum.CenterDialogType centerDialogType, Function showFunction, Function hideFunction)  
AddKey(string key)  
AddSelectionParent(string selectionName, Instance selectionParent)  
AddSelectionTuple(string selectionName, Tuple selections)  
AddSpecialKey(Enum.SpecialKey key)  
BroadcastNotification(string data, int notificationType)  
ClearError()  
CloseInspectMenu()  
CloseStatsBasedOnInputString(string input)  
ForceTenFootInterface(bool isForced)  
[GetBrickCount()](#getbrickcount)  
GetClosestDialogToPosition(Vector3 position)  
GetEmotesMenuOpen()  
GetErrorCode()  
GetErrorMessage()  
GetErrorType()  
GetGameplayPausedNotificationEnabled()  
GetGuiInset()  
GetGuiIsVisible(Enum.GuiType guiType)  
GetInspectMenuEnabled()  
GetNotificationTypeList()  
GetResolutionScale()  
GetSafeZoneOffsets()  
GetScreenResolution()  
GetUiMessage()  
InspectPlayerFromHumanoidDescription(Instance humanoidDescription, string name)  
InspectPlayerFromUserId(int64 userId)  
InspectPlayerFromUserIdWithCtx(int64 userId, string ctx)  
IsMemoryTrackerEnabled()  
IsTenFootInterface()  
OpenBrowserWindow(string url)  
OpenNativeOverlay(string title, string url)  
RemoveCenterDialog(Instance dialog)  
RemoveKey(string key)  
RemoveSelectionGroup(string selectionName)  
RemoveSpecialKey(Enum.SpecialKey key)  
Select(Instance selectionParent)  
SetEmotesMenuOpen(bool isOpen)  
SetGameplayPausedNotificationEnabled(bool enabled)  
SetGlobalGuiInset(int x1, int y1, int x2, int y2)  
SetHardwareSafeAreaInsets(float left, float top, float right, float bottom)  
SetInspectMenuEnabled(bool enabled)  
SetMenuIsOpen(bool open, string menuName = "default")  
SetSafeZoneOffsets(float top, float bottom, float left, float right)  
SetUiMessage(Enum.UiMessageType msgType, string uiMessage = "errorCode")  
ShowStatsBasedOnInputString(string input)  
[ToggleFullscreen()](#togglefullscreen)  
ToggleGuiIsVisibleIfAllowed(Enum.GuiType guiType)

## Events

[MenuOpened()](#menuopened)  
[MenuClosed()](#menuclosed)

### GetBrickCount

`RobloxScriptSecurity`  
Returns the place's brick count.

### ToggleFullscreen

`RobloxSecurity`
Toggles fullscreen mode.

### MenuOpened

Fires whenever Roblox's CoreGui menu is opened.
```
game:GetService("GuiService").MenuOpened:Connect(function()
    print("Menu has been opened!")
end)
```

### MenuClosed

Fires whenever Roblox's CoreGui menu is closed.
```
game:GetService("GuiService").MenuClosed:Connect(function()
    print("Menu has been closed!")
end)
```