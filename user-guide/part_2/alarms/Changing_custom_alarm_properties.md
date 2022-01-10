## Changing custom alarm properties

In this section:

- [Adding a custom alarm property](#adding-a-custom-alarm-property)

- [Deleting a custom alarm property](#deleting-a-custom-alarm-property)

- [Editing custom alarm properties](#editing-custom-alarm-properties)

> [!TIP]
> See also:
> <https://community.dataminer.services/video/alarm-console-adding-extra-properties-on-alarms/>

### Adding a custom alarm property

1. Right-click an alarm in the Alarm Console, and select *Properties*.

2. Go to the *Custom* tab.

3. Click the settings button in the lower left corner, and select *Add*.

4. Enter a name for the new custom property.

5. If alarms should be updated when the value of this property changes, make sure *Update alarms on value changed* is selected; otherwise make sure this checkbox is cleared.

6. Specify a property format.

    There are three possibilities:

    - Select “No value format” if you do not want to restrict the property value in any way.

    - Select “Format (regular expression)” to restrict the property value by means of a regular expression.

    - Select “Possible values” and specify a number of allowed values.

### Deleting a custom alarm property

1. Right-click an alarm in the Alarm Console, and select *Properties*.

2. Go to the *Custom* tab.

3. Select the property you want to delete.

4. Click the settings button in the lower left corner, and select *Delete*.

> [!CAUTION]
> Be careful when deleting alarm properties. If you delete an alarm property, it will be removed from all alarms.

### Editing custom alarm properties

If an alarm tab contains columns displaying custom alarm properties, the values of those properties can be changed as follows:

- In a column with a custom alarm property, click the pencil next to the property value and enter the new value.

    > [!NOTE]
    > While you are editing an alarm property, the Alarm Console tab page will be frozen. In the header of the tab page, you will notice the word “(Frozen)” next to the name of the tab page.

If no such columns are displayed, it is still possible to change any available custom alarm properties as follows:

1. Right-click an alarm in the Alarm Console and select *Properties*.

    Alternatively, to view properties for several alarms at a time, select several alarms by holding the *Ctrl* key while you click them, then right-click one of the alarms and select *Properties*.

2. In the *Properties* dialog box, select the *Custom* tab.

3. Enter the property value you want and click *OK*.

    > [!NOTE]
    > If you selected several alarms, and these have different property values, the value field will display *(Multiple Values)*.

You can also edit advanced settings of a custom alarm property, such as the property format:

1. Right-click an alarm in the Alarm Console, and select *Properties*.

2. Go to the *Custom* tab.

3. Select the property you want to edit.

4. Click the settings button in the lower left corner, and select *Edit*.