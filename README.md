# FTView-SE-Popups
Backup file is Network Station, FTView SE V15

How to create popups in FTView SE similar to RSView32.

This topic comes up enough to post an example.  Common request is how to open a display based on a tag value.  Since FTView SE is Client/Server even when operating as Local Station or Network Station the Events are not able to open displays since Events execute at the Server level.

This example uses a window that is made invisible when the display is opened with VBA. "Me.Visability = false".  On that display you place the tags you want to monitor and attach VBA code to the change events for the objects (numeric display, etc) on the display.
Within that VBA code you open the displays that are needed.

The initial diplays are opened using the startup macro that is configured to be called by the PopupDemoClient.CLI configuration file.  Will add additional information in the future.
Hope it helps solve any issues related to this.


