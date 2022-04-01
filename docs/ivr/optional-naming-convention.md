The main **IVR Datatable** shows all IVR’s found in your [RingCentral®](https://ringcentral.com) account and any values pulled from the IVR names via the **Optional Naming Conventions**. These key:value pairs are used to create custom columns of data in the IVR section data table that allows for grouping/filtering based on unique business-specific logic.

## Custom Columns and Values
Any columns of data pulled by the Optional Naming Convention feature will be displayed after the first four columns in the datatable and will also be indicated by a Hit the ![Star icon](../assets/star.svg "Star icon") star icon after the column title in the IVR datatable.

## Using the Optional Naming Conventions

Use the following pattern when naming your IVR’s inside of the RingCentral service portal to take advantage of this feature:

<pre><code>ivrname-key1:value1,key2:value2,key3:value3,key4:value4,key5:value5</code></pre>

*(64) character maximum, including spaces and punctuation. You may specify up to (5) custom key:value pairs separated by commas.*

The above pattern would produce an IVR named "ivrname" and then five new custom columns would be created. The custom columns would be named after the key names, "key1" for example, and the data underneath would be the values, "value1" etc... 

* After naming your IVR’s inside of the RingCentral service portal, login back into IVR Orchestrator and/or reload the IVR Datatable to see your changes.

* You should now see you IVR(s) with **Custom Columns** and values that you identified with the Optional Naming Conventions.