# $${\color{lightgreen}TestRail \space \space Test \space \space Plans \space \space and \space \space Test \space \space Runs}$$

# Overview

- ## The difference between a Test Run and a Test Plan

A **Test Run** would usually encompass one or two tests being done for a JIRA bug or case that involves a small scope.

A **Test Plan** would usually encompass a series of tests (at least 2 or more) for a project.

A **Test Plan** will always have **Test Runs** within it, while **Test Runs** do not necessarily have to be in a **Test Plan**.

- ## Test Run

A **Test Run** consists of individual tests for each case that is added and is an actual test you are conducting.

TestRail provides a two-step procedure for test execution. First, add the test run and then execute the test run. **Add Test Run** is simply pulling the existing test cases, as the test run is where the tester can execute those based on priority. For most projects, you will most likely start multiple test runs for a particular test suite over time. You can have multiple test runs for a particular test suite active at the same time. This can make sense if you want to execute a particular test suite for multiple configurations (such as different operating systems). You can then start a test run for each different configuration you want to test against.

You can add a test result and change the status of a test either by clicking the **Add Result** button on the test page or by changing it directly on the run page.

The following test statuses are available by default:
**Untested:** By default, new tests have the status Untested. Once a test result has been added, it can never receive the Untested status again.
**Passed:** A test is marked as Passed when a tester verifies the test steps and the expected results.
**Failed:** A tester marks a test as Failed if one of the specified test steps resulted in an error or if the expected result differs from the actual test result.
**Retest:** If a developer or tester determines that a test should be tested again, she marks the test as Retest. If a test originally failed and the developer fixed the problem, the developer can mark it to be retested.
**Blocked:** The Blocked status is used to signal that a test cannot be executed currently because of some external dependency (such as a bug that needs to be fixed before being able to complete to test). It is often used in combination with the Retest status.

Once a test run has been completed, you can close it from the run’s edit page. Tests of a closed run cannot be edited or changed, making it ideal for archiving test runs. Additionally, if you change any of the associated cases’ attributes (such as the expected result), the change won’t be applied to the closed and archived run.

- ## Test Run

When you need to manage multiple test runs and configurations for a single project, TestRail’s test plans come in handy. A test plan allows you to start multiple test runs at once if you want to test against multiple configurations. A configuration can be anything you need to test your projects against, such as different operating systems or web browsers. 

To create a test plan, simply click the **Add Test Plan** button from the **Test Runs & Results** page. Just like you do with a single test run, you can configure all properties of the test runs such as the name, the cases you want to include, and so on.

You often have to test a specific test run against multiple configurations such as operating systems or web browser versions. To make creating a separate test run for each configuration combination easier, you can specify and select all configurations for your test runs within a plan. To do this, simply click the **Select Configurations** link of a run and select or add your configurations.

$${\color{green}**────────────────────────────────────────────────────────**}$$

# Add Test Plan

1. Go to **Test Runs & Results** tab and click on the **Add Test Plan** button present on the right side
2. On the **Test Plan** page, enter the **Name**, **Milestone**, and **Description**
3. Following the instructions displayed in the advisory message, click the **Add Test Run(s)** button from the right sidebar
*(This will add available test runs)*
4. Click on the **Configurations** button to configure test runs
5. The **Select Configurations** pop-up will display the details of the available configurations. If the required configuration is not present, a new configuration can be added by clicking on the **Add Group** or **Add Configuration** link present in the pop-up.
6. Enter the name and click on **Add Group/Configuration** and after that click the **OK** button
7. The selected **Configuration** will be displayed against each **Test Run**. Click on the **Add Test Plan** button
8. After doing so, the newly created **Test Plan** will be displayed

$${\color{green}**────────────────────────────────────────────────────────**}$$

# Add Test Run

1. Go to the **Test Runs & Results** tab
2. Click on the **Add Test Run** button present in various places
3. The **Select Test Suite** pop-up will be displayed, select the test suite to include in the test run, then click the **OK** button
4. The **Add Test Run** page will be displayed, where the following information can be input: **Name**, **Milestone**, **Assigned To**, and **Description**
5. When selecting test cases to add to the **Test Run**, there are two options:
    - **Include all test cases:** Select this option to include all test cases in this test run. If new test cases are added to the repository, they are also automatically included in this run. 
    - **Select specific test cases:** Select test cases to include in this test run. New test cases are not automatically added to this run. When this option is selected, the following additional steps must be performed:
      - Click on the **change selection**
      - This opens the **Select Cases** wizard with all available test cases. The entire section or specific test cases from each section can be selected. Click the **OK** button to submit the selection.
6. The number of attached test cases is displayed beside the **change selection** option. Click the **Add Run** button
7. The test run will be successfully created and display a pie chart and test cases in the **Test Runs & Results** tab

$${\color{green}**────────────────────────────────────────────────────────**}$$

# Execute Test Run

1. Go to the **Test Runs & Results** tab
2. Click on the name of the test run to be executed
3. In the **Test Cases** section of the **Test Run** UI, select the title of a test case in **Untested** state
4. Follow the testing steps displayed in the **Steps** section
5. Click the **Add Result** button
6. In the **Add Result** pop-up, select the relevant test status, and click the **Add Result** button
7. Complete the previous process for the additional test cases in the **Untested** state

$${\color{green}**────────────────────────────────────────────────────────**}$$

# Rerun Test Run

1. While on the **Test Run** UI, click the **Rerun** button present in the toolbar
2. The **Select Tests** wizard, as shown in the following screenshot, will be displayed, allowing the tester to select the test cases based on the status of the previous test result
3. After selection, click the **OK** button
4. After clicking the **OK** button, the **Add Test Run** page is displayed where the tester should enter the following information:
    - **Name**
    - **Milestone**
    - **Assigned To**
    - **Description**
5. By default, the second test case selection option is selected. The number of test cases included is visible as well. Click on the **Add Run** button
6. After clicking the **Add Test Run** button, the pie chart and test cases of the newly created test run are displayed in the **Test Runs & Results** tab





