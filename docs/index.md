![IVR Orchestrator Logo](assets/ivrorchestrator-icon.svg "IVR Orchestrator Logo")

[IVR Orchestrator](https://ivrorchestrator.ps.ringcentral.com) provides bulk orchestration of IVR prompt media across multiple IVR’s in your [RingCentral®](https://ringcentral.com) account. The IVR prompt is the media that callers hear when calling an IVR before any key presses are performed. A summary of available features includes:

* **Bulk orchestration of IVR prompt media** across multiple IVR’s.
* **Schedule and combine prompts** to start/end on a specific date/time.
* Tag IVR names with custom values to **group and filter by business-specific logic** for easier bulk editing.
* **API integration** to your RingCentral media library and IVR’s.
* Customizable **role-based access and granular permissions** control.

See the **quick start** below or visit the [user guide](general/profile-menu) for full documentation.

# Quick Start

## Requirements

Chrome or Firefox web browser and a [RingCentral®](https://ringcentral.com) account with [Multi-Level IVR's](https://support.ringcentral.com/article/6562.html) enabled.

## Logging In

Log in to [IVR Orchestrator](https://ivrorchestrator.ps.ringcentral.com) using your [RingCentral®](https://ringcentral.com) credentials at the following URL:

> [https://ivrorchestrator.ps.ringcentral.com](https://ivrorchestrator.ps.ringcentral.com)

*Your RingCentral account administrator will need to enable access to this application for the role of your RingCentral user (see the users section below).*

New accounts automatically receive a **free 14-day trial period** upon first login. After the trial period expires, *you must contact your Account Executive or Sales Representative to purchase a subscription* for your account.

## IVR

The IVR section of this application displays a list of all IVR’s present in your RingCentral account. The list of IVR’s can be filtered to create a group that can be used to scope bulk management operations.

IVR prompts can be applied to IVR's immediately on an individual basis or in bulk, or they can be scheduled for deployment at a specified start/end date/time. Clicking on the name of any IVR in the data table will allow you to see the prompt media currently in use for the IVR as well as any upcoming scheduled prompts.

This application takes the scheduled prompt media and combines it with the default prompt media into a single audio file that can be dynamically managed and deployed to the RingCentral platform for each IVR. Scheduled prompts are played in the order you specify and the default prompt media is heard last.

*[Multi-Level IVR's](https://support.ringcentral.com/article/6562.html) must be implemented on the account to use this application.*

## Scheduling Prompts

Scheduling a prompt allows you to define a start and end date and time during which the prompt should be active.  You may create up to five (5) additional prompts in addition to the default prompt media. Any prompt can become a scheduled prompt by defining a start and end date within the IVR Prompt Media's configuration.

* Be aware when scheduling prompts across IVR’s in different time zones or site time formats (12h or 24h). For example, if you are bulk editing IVR’s across both the central and mountain time zones to schedule a prompt, and specify 3pm as the start time, it will be scheduled as 3pm central time and 3pm mountain time (no localization is performed).

Learn more about [Scheduling IVR Prompts](ivr/ivr-editing) for IVRs in your RingCentral Office account.

## Optional Naming Convention

IVR’s using the optional naming convention described below are further recognized by this application. These values are used to create custom columns in the IVR section data table that allows for grouping/filtering based on unique business-specific logic.

Use the following pattern when naming your IVR’s inside of the RingCentral service portal to take advantage of this feature:

<pre><code>ivrname-key1:value1,key2:value2,key3:value3,key4:value4,key5:value5</code></pre>

Custom columns created in this manner will be indicated by a star icon after the column label in the IVR datatable.

*(64) character maximum, including spaces and punctuation. You may specify up to (5) custom key:value pairs separated by commas.*

Each key:value pair represents an individual column in the IVR section data table. The key is the column heading and the value is the cell content. For example, you may have stores organized by state, region, district, etc. This could be modeled using the following the IVR naming convention example:

<pre><code>mainStoreIVR-state:CO,region:12,district:4</code></pre>

This allows bulk operations to be executed across user-defined datasets, for example changing the IVR prompts on all stores/locations in region 12.

Learn more about [Optional Naming Conventions](ivr/optional-naming-convention) feature.

## Media

Media refers to the actual audio files that callers hear when interacting with an IVR. The media section of this application displays a list of all media present in your RingCentral account. You may also add new media and remove existing media.

MP3 and WAV file types are supported. Multiple files can be uploaded simultaneously (bulk upload).

This section is fully integrated to the media library in your RingCentral account:

* Media imported into this application will appear in the RingCentral account media library.
* Media added directly to the RingCentral account media library will appear in this application.
* Deleted media will be removed from both this app and the RingCentral Office account media library.

Any media that is present can be used for orchestration activities across a single or multiple IVR prompts.

Learn more about [Importing New Media](media/import-new-media) and how you manage audio files with IVR Orchestrator.

## Users

The users section allows you to define which roles from your RingCentral account will have access to this application and what permissions the users having those roles will be granted. It also shows what users from your account have logged into the application.

A list of all roles present in your RingCentral account is automatically populated into the roles section. Enable a specific role with permissions to give its users’ access to this application.

The built-in super admin role is hardcoded with permanent RW access to avoid the potential of accidentally getting locked out. *A user with a* **super admin** *role on the RingCentral account must perform the initial role-enablement for other users this application.*

Permissions can be set for each existing role. You may grant read-only or read-write access to each individual section of this application to any given role.

Learn more about [Editing Role Permissions](users/editing-role-permissions) and enabling access for other user roles.


## Orchestrating Your First IVR Prompts

The first step to orchestrating your IVR prompts and creating scheduled media prompts is selecting which IVRs to edit. You may edit a single IVR or many at once by selecting several IVRs in the IVR data table. To add new media as a scheduled media prompt for one or more IVR(s), you will need to choose the media file, idenitfy start and end dates if needed, and place it in the desired position within the scheduled media order.

*Tip: Before orchestrating your first IVR scheduled media prompts, it is best to ensure any media you intend to use is uploaded and all IVRs that you want to edit have default prompt media.*

1. Select the IVRs you want to edit and then click the **Edit** button.
2. Click **New Prompt** button to open the **New Prompt Dialog Menu**.
3. Select the position in the scheudled media order for this item. *Default is first available position and items will drop in order if a position is empty.*
4. Choose the media file that will be used for the prompt media.
5. Add a start and end date if needed, or select **start now** and **no end date**.
6. When prompt configurations are finalized, click the **Create** button.
7. A success or error confirmation dialog will confirm final results.
8. Click the **Sync Changes** button to save edits and to apply your IVR prompt settings.

You may add new, remove and rearrange the order of scheduled media items but the system will always take-in account each IVR's configuration when bulk editing and creating the **combined prompt media files** when syncing your changes.

#  Wrapping Up

The essential item to remember when using IVR orchestrator is the **combined prompt media files** may differ between IVRs after edits due to different prompt media being used, but all configurations will remain dynamically managed by this application. Any scheduled start and end dates will still change the combined media file for an IVR prompt when they occur and the application will automattically shuffle the prompt media depending on your settings.

Below is collection of useful tips and tricks that will help guide you on your IVR orchesatration journey.

## Inital Setup Guidance

* [Multi-Level IVR's](https://support.ringcentral.com/article/6562.html) must be implemented on the account to use this application.

* A user with a* **super admin** *role on the RingCentral account must perform the initial role-enablement for other users of this application.

* RO is read-only access or view mode. The users of the role type cannot make any edits if RO is enabled for that section of the app.

* RW is read-write or edit mode. Users of that role type can change settings in that section of the app.

## Tips on Editing IVR Prompts

* Before orchestrating your first IVR scheduled media prompts, it is best to ensure any media you intend to use is uploaded and all IVRs that you want to edit have default prompt media.

* A combined prompt media file will be present if the IVR Prompt has scheduled prompt media and is being dynamically managed by this application.

* Be aware when scheduling prompts across IVR’s in different time zones or site time formats (12h or 24h). For example, if you are bulk editing IVR’s across both the central and mountain time zones to schedule a prompt, and specify 3pm as the start time, it will be scheduled as 3pm central time and 3pm mountain time (no localization is performed).

* Deleting and editing schedule prompt media and default media will require you to **Sync Changes** before your edits are applied to the IVR(s)

## Prompt media file notes

* The **combined prompt media files** can be found in the media section of this app and in your RingCentral account after syncing changes.

* Media imported into this application will appear in the RingCentral account media library.

* Media added directly to the RingCentral account media library will appear in this application.

* Deleted media will be removed from both this app and the RingCentral Office account media library.

* Hit the 'play' icon next to any audio file to preview it.

