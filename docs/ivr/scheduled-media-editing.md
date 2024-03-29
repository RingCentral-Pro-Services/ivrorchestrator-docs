Scheduling prompt media allows you to add prompt media that will play automatically in the order that is listed under the scheduled media section for the IVR. You may also define a start and end date range during which the specific scheduled prompt should be active or inactive. 

These features can be very useful when needing to change many IVRs, and their prompts, at one time or to schedule prompts to play at certain times and dates.

Learn more about [Bulk Editing Scheduled Prompts](ivr/bulk-ivr-editing) for many IVRs at one time.

*A **combined prompt media file** will be present if the IVR Prompt has scheduled media that is currently being dynamically managed by this application.*

![Scheduled prompts and combined media file](../assets/scheduled-prompt-media.png "Scheduled prompts and combined media file")

## Schedule New Media Prompts

To add new media as a scheduled media prompt for an IVR, you will need to choose the media file, identify start and end dates if needed, and place it in the desired position within the scheduled media order.

1. Click **New Prompt** button to open the **New Prompt Dialog Menu**.
2. Select the position in the scheduled media order for this item. *Default is first available position and items will drop in order if a position is empty.*
2. Choose the media file that will be used for the prompt media.
3. Add a start and end date if needed, or select **start now** and **no end date**.
4. When prompt configurations are finalized, click the **Create** button.
5. A success or error confirmation dialog will confirm final results.

* After any actions to an IVR Prompt, the application will require you to **Sync Changes** or you will lose your edits. 

After adding scheudled prompt media, you may drag to rearrange the items to the desired positions using the Move icon ( ![Move icon](../assets/move.svg "Move icon") ) located on the left side of the scheduled prompt rows. 

*You may schedule up to five (5) additional prompts in addition to the default prompt media.*

* Be aware when scheduling prompts across IVR’s in different time zones or site time formats (12h or 24h). For example, if you are bulk editing IVR’s across both the central and mountain time zones to schedule a prompt, and specify 3pm as the start time, it will be scheduled as 3pm central time and 3pm mountain time (no localization is performed).

## Combined Prompt Media File

When IVR Orchestrator is used to manage an IVR's prompt media, it will generate a **combined prompt media file** that is dynamically managed and deployed to the IVR. This file can be found next to the 'Scheduled Media' section title contained within the blue rectangle similar in style to a button. 

Once deployed, this file can be found in **Media** of this app and in your [RingCentral®](https://ringcentral.com) account.

* Hit the ![Play icon](../assets/play.svg "Play icon") play icon next to the file to preview the combined prompt media file.

*Combined audio files are named with the following format, 'z + custom-ivr-prompt- + date in numerical format.mp3'. The z in-front ensures these files are at the end of your media files list in the RingCentral admin portal.*