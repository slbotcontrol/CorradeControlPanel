# Corrade Control Panel Release Notes

**[Note:]** The `Corrade Control Panel` is still under development and subsequent releases will follow quickly. Consider this release an `Alpha` release intended for internal testing only.

`Corrade Control Panel` is an LSL script library to control `Corrade` bots from an LSL script.

The `Corrade Control Panel` is a scripted in-world object that acts as a bridge between your `Corrade` management scripts and your `Corrade` bots. The control panel communicates with your bots using the `Corrade API` and an HTTP server listening to events.

## Deployment

Download the `CorradeControlPanel.lslo` script, the `Configuration` notecard, and the `header.lsl`.

In Second Life create a new script named `CorradeControlPanel` and copy the contents of `CorradeControlPanel.lslo` into this new script. Similarly, create a new notecard named `Configuration` and copy the contents of `Configuration` into this new notecard.

Edit the `Configuration` notecard and replace `your-api-key` in the line `LB_API_KEY = your-api-key` with your `Corrade` developer API key.

You do not need to edit the `CorradeControlPanel` script.

Create a new object, right click the object and select `Edit`.

Copy the `CorradeControlPanel` script and `Configuration` notecard into the `Contents` tab of the new object.

Create a new command and control script or modify an existing `SmartBots TotalControl` script. Include the `header.lsl` control codes in your command and control script.

Copy your `Corrade` command and control script into the `Contents` tab of the new object. If you do not have a command and control script then you can use one of the examples described below.

Close the Edit window.

## Corrade Command and Control Script Examples

`Corrade Control Panel` acts as a bridge between your command and control scripts and your `Corrade` bots. Included in this release are several example command and control scripts. To deploy one of these command and control scripts, first edit the script and configure your `Corrade` bot name and bot secret. 

Once configured with the bot name and secret, copy the example `Corrade` command and control script into the `Contents` tab of the `Corrade Control Panel` object.

**[Note:]** Some example command and control scripts may have additional variables that need to be configured. For example, the `sit_on_payment` example needs to be configured with the UUID of the object you want your bot to sit on when payment is received.
