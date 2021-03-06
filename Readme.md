# College Credits Tracker Task Pane Add-in Sample for Excel 2016

_Applies to: Excel 2016_

This task pane add-in shows how to create a college credits tracker using the JavaScript APIs in Excel 2016. It comes in two flavors: text editor and Visual Studio.

![College Credits Tracker Sample](images/CollegeCreditsTracker_tracker.PNG)

## Try it out
### Text editor version

The simplest way to deploy and test your add-in is to copy the files to a network share.

1.  Deploy the files in the Text Editor version to a server of your choice.
2.  Edit the \<SourceLocation\> and \<Urls\> elements of the manifest file so that it points to the hosted location from step 1. (i.e. https://localhost)
2.  Create a folder on a network share (for example, \\\MyShare\CollegeCreditsTracker) and copy all the files in the Text Editor folder.
3.  Copy the manifest (CollegeCreditsTrackerManifest.xml) to the network share (for example, \\\MyShare\MyManifests).
4.  Add the share location that contains the manifest as a trusted app catalog in Excel.

    a.  Launch Excel and open a blank spreadsheet.

    b.  Choose the **File** tab, and then choose **Options**.

    c.  Choose **Trust Center**, and then choose the **Trust Center Settings** button.

    d.  Choose **Trusted App Catalogs**.

    e.  In the **Catalog Url** box, enter the path to the network share you created in step 1, and then choose **Add Catalog**.

   f.  Select the **Show in Menu** check box, and then choose **OK**. A message appears to inform you that your settings will be applied the next time you start Office.

5.  Test and run the add-in.

    a.  In the **Insert tab** in Excel 2016, choose **My Add-ins**.

    b.  In the **Office Add-ins** dialog box, choose **Shared Folder**.

    c.  Choose **College Credits Tracker Sample**>**Insert**. The add-in opens in a task pane to the right of the current worksheet, as shown in the following figure.

   ![College Credits Tracker Sample](images/CollegeCreditsTracker_taskpane.PNG)

    d.  Click the **Create College Credits Planner** button. This create the college credits tracker in the active sheet as shown in this diagram.

  ![College Credits Tracker Sample](images/CollegeCreditsTracker_tracker.PNG)

    e.  Add some courses using the **Add a course** tab and see how the data and the chart changes dynamically.

### Visual Studio version
1.  Copy the project to a local folder and open the Excel-Add-in-JS-CollegeCreditsTracker.sln in Visual Studio.
2.  Press F5 to build and deploy the sample add-in. Excel launches and the add-in opens in a task pane to the right of a blank worksheet, as shown in the following figure.

  ![College Credits Tracker Sample](images/CollegeCreditsTracker_taskpane.PNG)

3.  Click the **Create College Credits Planner** button. This create the college credits tracker in the active sheet as shown in this diagram.

  ![College Credits Tracker Sample](images/CollegeCreditsTracker_tracker.PNG)

4. Add some courses using the **Add a course** tab and see how the data and the chart changes dynamically.


### Learn more

The Excel JavaScript APIs have much more to offer you as you develop add-ins. The following are just a few of the available resources.

1.  [Excel Add-ins programming overview](https://github.com/OfficeDev/office-js-docs/blob/master/excel/excel-add-ins-programming-overview.md)
2.  [Snippet Explorer for Excel](http://officesnippetexplorer.azurewebsites.net/#/snippets/excel)
3.  [Excel Add-ins code samples](https://github.com/OfficeDev/office-js-docs/blob/master/excel/excel-add-ins-code-samples.md)
4.  [Excel Add-ins JavaScript API Reference](https://github.com/OfficeDev/office-js-docs/blob/master/excel/excel-add-ins-javascript-reference.md)
5.  [Build your first Excel Add-in](https://github.com/OfficeDev/office-js-docs/blob/master/excel/build-your-first-excel-add-in.md)