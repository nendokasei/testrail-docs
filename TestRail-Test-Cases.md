# Overview

A test case consists of a description, the test's prerequisites (i.e. Areas Affected, Preconditions, Additional Information), list of test steps, and the expected result. The test case confirms a specific functionality, documents a task, verifies a project artifact, and can be verified by a tester.

In the test cases tab, test cases are organized under different sections and subsections to allow for ease of access. 

Commonly used test case Types include:
- **Functional:** Manual test with step-by-step instructions and a list of expected results for each of those steps.
- **Automated:** Perl script that simulates user interaction. Results will be Pass or Fail.
- **Duplicate:** For test cases that duplicate an existing case.
- **Obsolete:** A test case that is no longer applicable to the product.
- **Exploratory:** This test is for an Exploratory template.  Mostly for a new feature. Click and see what happens.

The 2 default test case Templates are:
- **Exploratory Session:** Exploratory Session template uses large text fields where you can define your Charter and Goals, add document notes, attach screenshots, and upload log files as you carry out your exploratory sessions.
- **Test Case:** The Test Case template allows you to delineate individual Steps along with the Expected Result for each step while providing areas to specify Preconditions, Test Steps, and Expected Results.

---

## Add Test Cases

1. Go to **Test Cases** tab and click on the **Add Case** link
2. This opens the **Add Test Case** form where a **Title** can be entered
3. **Section**, **Type**, **Template**, **Type**, **Automation Type**, and **Priority** are mandatory fields and are selected by default
*These fields can be modified to suit the needs of the case being created.*
4. Complete the **Summary** and **Areas Affected** fields
5. Under the **Steps** section, click **Add the first step.**
6. Input the test step details in the first field and the expected result in the second field
7. To add additional steps, click **Add Step** beneath the last created step
8. Click on the **Add Test Case** button
9. A success message is displayed upon the successful addition of the created case, along with the **Add Another** link

---

## Edit Test Cases

1. Click on the name of the test case to open the details
2. Click on the **Edit** button present at the top right of the page
3. After editing, click on the **Save Changes** button

---

## Add Table

1. To add a table to a text box, click on the **Table** icon present in the top right of the text box
2. This will open the **Add Table** pop up where the table template can be modified. The right **+** button will add a new column, while the down **+** symbol will add a new row
3. Click on the **Add Table** button to add the table template into the text box
4. Once the table template is added to the text box, the desired contents of the newly created table can be input

---

## Add Image

1. To add an image to a text box, click the **Image** icon present at the top right of the text box
2. A pop-up will display where one or more images can be added. Multiple options are available for adding images, such as:
- **ALT+PrntScr** to take screenshot and then press **CTRL + V** to paste it directly
- A previously saved image can be added to the **Add Image** pop-up by clicking on the space that says **"Drop images here to embed, or click to browse."**
- By clicking the **Remove** link, the image will be removed
3. By clicking the **Add Images** button, the image(s) will be added to the text box
4. Click on the **Save Test Case** button

---

## Copy/Move Test Cases

### Copy/clone a single test case within the same project

To copy or clone a single test case, you can drag & drop the case from the test case repository list, or simply press and hold the **Shift** key during the operation. To do this, simply drag the little grip icon on the left of the checkboxes.

You can also copy or clone whole sections or subsections of test cases in the sidebar. If you want to copy/clone test cases in the sidebar, simply press and hold the **Shift** key while selecting a section or subsection and drag the section to where you would like to copy it or use drag & drop.

### Copy/clone multiple test cases within the same project

You can also copy/clone multiple test cases by selecting multiple test cases by checking the boxes on the left-hand side of the test case table first. Then drag & drop as you would with a single test case, and select **“Copy here”**. Alternatively, you can click and hold the **Shift** key before dragging your selected test cases to automatically make a copy of them.

### Copy/clone a test case section within the same project

To copy or clone an entire section within a test suite, you can drag & drop a section/s or simply press the **Shift** key before and during the operation in the sidebar.

### Copy/clone from another test suite (for projects with multiple test suites) and different projects

If you want to copy or clone test cases or entire sections from another test suite, simply open the **Copy or Move Cases** dialog from the toolbar of a test suite (it’s the little icon with two sheets of paper in the toolbar). You can also use this dialog to duplicate entire test suites.

---

## Import Test Cases From CSV

### Prepare Your Source File to Import

##### Prepare your source file to import
You can do this in Excel under **File > Save As**, and select CSV (Comma delimited) (*.csv) as the file type. This will save your test cases as a CSV file which you can import into TestRail.

### Rules for CSV file

When using the **Test Case (Steps)** template, each test case that has multiple steps should span multiple rows, where all of the standard fields, the first step, and the expected result are defined in the first row, and each additional step and the expected result should be on a separate row in the same column. The CSV file should have data in the first sheet only. 1st row should have header names in different columns and the next onwards data should represent each column. Please note, 1st row will be mapped with different fields of Test Case Forms while importing. Required fields must be mapped with a column of the CSV sheet and it shouldn’t be blank. Otherwise, the system will generate an error message of unsuccessful import.

### Importing your CSV to TestRail

To start the import process, first, navigate to the test case repository in TestRail you would like to import into. This may be the **Test Cases** tab of a single repository project, or within a **Suite** or **Baseline** if you’re using one of the alternative project types.

You can then open the **Import CSV** dialog in the toolbar of the test suite/test case repository using the **Import** icon (the window with the green arrow pointing in).

The CSV import allows you to migrate existing test cases using a simple wizard dialog. TestRail supports all typical CSV variants, the conversion of common character encodings, and various CSV formats. You can upload your CSV file and configure various file-related options in the first wizard step.

#### Import Step 1 - File Selection and Options

You’ll see several options present on the first page of the import wizard:

First, under **File**, select the CSV file you want to import. Below that, the option for **Format & Mapping** will let you select a configuration file if you have one. If you do not have a configuration file, select **"Configure new mapping"** for the first import. After a successful import, you’ll be given the option to download the configuration file for the import, which will save all of the import configuration settings, allowing you to save time and effort when importing subsequent CSV files.

> [!NOTE]
> The upload size limit for CSV imports is 10MB. If your file is larger than 10MB, please split it into smaller files or remove any unnecessary data before importing.

In the **Advanced Options** section you will have a few additional settings to configure before continuing:

| `Option` | `Description` |
| --- | --- |
| **Import to** | The base section or folder you would like to add your test cases to. Sections defined on your test cases in the imported CSV file will be added as sub-sections under this section. By default, will select a blank value, which will add all defined sections as top-level, or they will be added to a generic “Test Cases” section if one is not defined in the CSV. |
| **Encoding** | The file encoding of the CSV file. Excel/Windows commonly uses Windows-1252 (Latin) for CSV files whereas most other tools (including Google Sheets) prefer the Unicode-compatible UTF-8 encoding. |
| **Delimiter** | The text character is used to indicate where information for the next cell should start. Standard CSV (short for Comma Separated Values) uses a Comma (,) but some sheets may be configured differently based on user preferences, how the file was created, or other factors. Generally, the comma will be the correct option. |
| **Start Row** | The index (starting at 1) of the row where TestRail should start looking for test cases in the CSV file. This can be used to ignore or skip lines at the beginning of the CSV file. |
| **Header Row** | Indicates if the start row of the content in the CSV file is a header row. A header row describes the CSV file and contains the identifiers used to match the relevant fields in TestRail to the column names. Excel or Google Spreadsheet documents usually have such a header row. |
| **Template** | The case template to use for the imported test cases. The template specifies the field layout and supported system/custom fields for the test cases. Depending on the template you are using, some additional formatting may need to be done to ensure compatibility with the selected template, most notably when using the Test Case (Steps) template. |

The first wizard step also allows you to upload a previously created configuration file (created at the end of the import process) with all import options of the previous import. This is useful if you need to import multiple CSV files with a similar or the same file layout.

After the settings configuration, click the **Next** button.

#### Import Step 2 - Column Mapping 

The next step to get your data imported is to map the columns of your spreadsheet to their respective fields inside TestRail. When you get to this step, the first option will be to specify whether test cases span a single row or multiple rows. TestRail differentiates between single- and multi-row case layouts for CSV files. A single-row layout means that every test case is represented by a single row or record in the CSV file. This is the standard layout for most CSV files.

If a test case spans or may span multiple rows/records in a CSV file, TestRail supports this by selecting the multi-row layout. When selected, you will also need to select the column that detects the start of a new test case (for example, an ID or Name/Title column which is unique per test case).

As mentioned, a multi-row layout is used for test cases with multiple individually defined steps and expected results and one row/record per step/expected result.

In the main section of the import dialog, on the left side, you’ll see a list of all of the column headings that the importer was able to find in your sheet. On the right side, you’ll see several dropdown fields showing the full selection of TestRail fields available for use in the project you’re importing to.

Select the relevant, matching field from within TestRail for each spreadsheet column heading. In some cases, you may have values in the spreadsheet that don’t directly match a TestRail field by name but would make sense to associate.

For example, if you plan to sort your test case repository by functional area of your product (in categories like “Installation”, “Authentication”, etc.) and you have a column in your spreadsheet with those types of categories, you can map that to the section field here to create those folders.

The last option in this step specifies if TestRail should ignore CSV rows/records without a valid, non-empty title column. It is recommended to keep this option enabled to filter out empty rows at the beginning/end of the CSV file or between regular test cases.

> [!TIP]
> When importing your test cases, you can have the system automatically create sections and subsections in your test case repository as part of the test case import process. During the import process, if you have a column that can match sections, it can be mapped to a section, and any values present in the spreadsheet that do not match an existing section will be created as a folder in your test case hierarchy.
> 
> If you’d like to create sub-sections, this can also be done by naming all sections and subsections, separated by a **>**
> 
> **Example** – There is a section column in an import file, one test case has a value of “Login”, which contains test cases related to the login screen and authentication. There is a separate mechanism used for a “Forgot Password” option with multiple test cases for this process that should be in a subsection of the login section. In this case, during the import, a user can set it up with the value **Login > Forgot Password.**
> 
> This can be extended with multiple subsections as needed:
> 
> Top Section > Sub-section 1 > Sub-section 2

#### Import Step 3 - Value Mapping

With your columns mapped to their respective fields, the next step will be to map the values of those fields to their corresponding values in the spreadsheet.

You should see all of the columns that were mapped to fields in the previous step, and if the field supports a drop-down or multi-select option, you will see the values present in the CSV on the left, and a series of menus allowing you to select the relevant field values from inside TestRail. If the values from the CSV match a field option exactly, they should be automatically linked, however, if you use different terms or values for certain fields, you may need to manually link them.

**Example:** TestRail by default defines priority using **Low**, **Medium**, **High**, and **Critical**. If your team is using something like numerical values or different terms for your priority definition, you’ll need to use the value mapping to select the most appropriate analog from the TestRail system. Note – it is also possible to customize the fields before importing to match your preferred nomenclature or add/remove field selections if required.

For all fields in this step, you also have the option to strip any HTML tags from the field values. This is useful if you’re importing from a separate tool that exports HTML tags in the CSV content.

#### Import Step 4 - Preview, Finalize, and Configuration Files

The final step will be to preview the import. TestRail will show you the general examples of how the first few test cases will appear during import. Once you’ve confirmed that all of the information appears correct, you can finish the process by clicking **“Import.”**

When completed, you’ll see a pop-up confirming that everything was successful, and provide you with a link to download the configuration file for the import that has been processed. This file can be loaded on the first wizard step in future imports, and will automatically pre-configure all wizard steps and import options to what was set throughout this import. This is especially useful if you need to import multiple CSV files with a similar or same layout. You can also share this configuration file with other team members if they will be performing similar imports.

---

## Import Cases From XML

### Importing Test Cases

You can fill a test suite with existing test cases and sections by loading an XML import file into TestRail. When you click on the import icon in the toolbar of a test suite (the icon with an arrow pointing to the left), the import dialog opens and you can select an XML file to import. In case you haven’t already added a test suite to import test cases to, please make sure to create a new (empty) test suite first.

### TestRail's Import Format

The import file must be given in a specific XML format which is outlined and explained in this section. The XML format represents a tree of sections, test cases, and subsections, just like the content of a test suite. The basic format of an import file looks as follows:

```
<?xml version="1.0" encoding="UTF-8" ?>
<sections>
  <section>
    <name>...</name>
    <description>...</description>
    <!--
    The test cases of the section. This is just a list of
    <case> elements plus fields such as title or type.
    This element is optional.
    -->
    <cases>
      <case>
        ...
      </case>
      ...
    </cases>
    <!--
    The subsections, if any. Can also contain test cases
    and further subsections etc. This element is optional.
    -->
    <sections>
      <section>
      ...
      </section>
      ...
    </sections>
  </section>
  ...
</sections>
```

> [!NOTE]
> To take a look at an actual TestRail XML file, you can just use the export feature of an existing test suite. The import and export functions use the same file format and taking a look at an actual example might help you better understand the file format. Note that the exported files have an additional top-level element which is automatically ignored when importing a file and can thus be omitted.

The above example explained how to express TestRail’s section tree structure in XML files. We will now take a look at how to specify all the additional fields of the element.

The element supports all properties of a test case in TestRail such as the title, estimate, priority, text fields, etc. A fully specified test case thus looks as follows:

```

...
<case>
  <title>Lorem ipsum dolor sit amet ... </title>
 
  <!-- The type of the test case. Please see your TestRail   
  installation for the supported types. -->   
  <type>Usability</type> 
 
  <!-- The priority of the test case, specified as a simple
  number. Please see your TestRail installation for the
  supported priorities. -->
  <priority>2</priority>
 
  <!-- The estimate of the test case, specified in seconds. -->
  <estimate>100</estimate>
 
  <!-- The milestone of the test case. Is looked up in the
  project you import the test cases to. -->
  <milestone>Beta 1</milestone>
 
  <!-- The references of the test case (a list of IDs, separated
  by comma or space). May be used to link the test case to external
  references (requirements or user stories, e.g.). -->
  <references>REQ-1, REQ-2</references>
 
  <custom>
    <!-- Custom fields go here -->
    ...
  </custom>
</case>
...
```

Note that all fields except the <title> are optional. TestRail will automatically choose a default value or leave a field empty if it’s missing.

---

## Export Cases to CSV/XML

### Export to CSV

To export the sections and test case details into a CSV file, select the **Export to CSV** option.

This opens the **Export to CSV** wizard. Selection of the content to be exported can be selected here, the user can select all sections or single/multiple sections to export.

Specific columns can be selected for export as well.

After selection, click on the **Export** button. After clicking the **Export** button, a CSV file containing all selected details will be downloaded.

### Export to XML

To export all details into XML, select **Export to XML**. It will directly download an XML file having all the details of test cases and sections.

An XML file would have a section tag and inside section cases and properties of cases.

