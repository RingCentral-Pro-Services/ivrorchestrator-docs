This application takes the all prompt media and combines it with the default prompt media into a single audio file that can be dynamically managed and deployed to the RingCentral platform for each IVR.

Scheduled prompts can be applied to IVR's immediately on an individual basis or in bulk, or they can be scheduled for deployment at a specified start/end date/time.

*[Multi-Level IVR's](https://support.ringcentral.com/article/6562.html) must be implemented on the account to use this application.*

Learn more about [Bulk Editing IVRs](ivr/bulk-ivr-editing).

## Editing IVR Prompts

There are several ways you can manipulate and edit the IVR Prompts. You may change the **Default Prompt Media**, add and remove **Scheduled Prompts**, add start/end dates, and manipulate the **Prompt Order**. 

* After any actions to an IVR Prompt, the application will require you to **Sync Changes** or you will lose your edits.

## Default Prompt Media

The default prompt media is the media that is assigned to the IVR by default from your RingCentral account IVR configuration. This media can be added and changed with the IVR Orchestrator, but it must have media present for this application to be able to add scheduled prompt media and sync the changes.

Learn more about [Default Prompt Media](ivr/bulk-ivr-editing).

## Scheduled Prompts

Creating new scheduled prompts is one of the primary ways to use the application. This area also identifies the **combined prompt media file** that is dynamically managed and deployed to the IVR(s) when using this application.

* A combined prompt media file will be present if the IVR Prompt has scheduled media that is dynamically managed by this application.

Click the **New Prompt** button in the upper right to add a new prompt to the scheudled media order.

Learn more about [Scheduling IVR Prompts](ivr/bulk-ivr-editing).

## Scheduled Media Order

The scheduled media order identifies the sequence in which the scheduled media files play. The prompts will play in the order 1,2, 3, 4, 5. The only exception is if your scheduled prompts have start and end times. If the scheduled prompt is not within it's time range, it will be excludued from the dynamically combined file.

## Edit or Delete Scheduled Media Items

To edit or remove a file in the scheduled media order, click the overflow icon on the far right of the item row athen choose **Edit** or **Delete** from the overflow dropdown menu.

*Deleting and editing prompt media will require you to **Sync Changes** before your edits are applied to the IVR(s)*

## Reording Scheduled Media Items

Each scheudled media item row can be moved and re-ordered within this list. Clicking and hold on the move icon, and then drag the item into the desired position.

*The combined prompt media file will always have the default prompt media as the last media file when combined with the scheduled prompts.*

## Syncing Changes

To sync edits and changes to an IVR Prompt, click the **Sync Changes** above the prompt media datatable. This will then combine all prompt media with the default prompt media into a single audio file that will be dynamically deployed to the IVR.

1. Click the **Sync Changes** button after making edits to an IVR Prompt.
2. Wait for fail or confirmation dialog for results.
3. If successful, the new combined media file will be deployed to the IVR Prompt and can now be dyncamially managed in this application.
