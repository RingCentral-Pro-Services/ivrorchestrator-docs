Bulk editing many IVRs is very similar to editing individual an IVR, but with a few key differences. To engage a bulk edit of many IVRs, select the IVRs to edit by clicking the checkboxes to the left of the IVR items in the IVR data table and clicking the **Edit** button.

* After any bulk actions to IVR Prompts, the application will require you to **Sync Changes** or you will lose your edits.

## Bulk Editing IVR Prompts

When bulk editing many IVRs and their prompt media, the system will look at each IVR's confgiuration. This means the **combined prompt media file** will be different for each IVR in your selection if their default media or scheduled media differs from one and another.

The default media and the scheduled media order will also reflect the different IVR prompt configurations in your bulk selections. Default media will be displayed as an **empty state** and scheduled media items will be shown as generic **Scheduled media found** row entries in the scheduled media rows if media is found. Due to current limitations we cannot show all prompt configurations for IVRs when bulk editing.

You can perform the same edit actions on a bulk selection that can be done on an individual IVR editing. Editing the **Default Prompt Media**, add and remove **Scheduled Prompts**, edit start/end dates for these prompts, and manipulate the **Prompt Order**. 

## Bulk Edit Default Prompt Media

Specific default media will not be shown for each IVR configuration when bulk editing but you may still edit this media during a bulk selection. When editing default media in bulk, you will be able to only select one specific media file for the entire selection. After editing, the choosen file will be shown until you sync and navigate away from the current bulk selection.

* Similar to individual IVR editing, each IVR in your bulk selection must have default media present before you can use this application to apply and sync scheduled media changes.

## Bulk Editing Scheduled Prompts

You may add new, remove and rearrange the order of scheduled media items but the system will always take-in account each IVR's configuration when bulk editing and creating the **combined prompt media files**. This means not all IVRs configs will have prompt media in all rows, even if prompt media order reflects the maximum of 5 row items including new scheduled media and **scheduled media found** items. Specific IVR configurations will logically rearrange scheduled prompt rows to fill empty spots lower in the media order list when a configuration has scheduled media missing for a specific row. 

* Combined prompt media files will differ between IVRs after a bulk edit, but all configurations will remain dynamically managed by this application and any scheduled start and end dates will still change the combined media file for the the IVR prompt when they occur.

*Tip: Double check that all IVRs have a default media file assigned in each IVR's prompt configuration before performing a bulk edit of scheduled media. This will ensure you don't encounter the 'default media required' error.*

## Bulk Delete Scheduled Media Items

You may remove any schduled media items when editing IVR prompt configurations in bulk, but take note that this will remove it from ALL IVR configs in your bulk selection.

* Scheduled media items will rearrange in the scheduled media order when items lower in the list are removed and item is above it.

*Deleting and editing prompt media will require you to **Sync Changes** before your edits are applied to the IVR(s)*
