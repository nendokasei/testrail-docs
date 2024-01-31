# Introduction to TestRail

TestRail is a web-based test case management tool that plays a vital role in the software testing ecosystem. It serves as a go-to platform for testers, developers, and team leaders alike, enabling them to efficiently oversee, monitor, and structure their software testing endeavors. With TestRail, team members can seamlessly create and input test cases, arrange them into test suites, execute comprehensive test runs, and closely monitor and analyze the results—all through an intuitive web-based user interface.

---

## The Dashboard

Upon logging into TestRail, your initial landing page is typically the dashboard. This central hub offers a comprehensive snapshot of your available projects, recent project activities, and your pending tasks.

When you choose to explore a specific project by clicking on its title, you seamlessly transition to the project view, arriving at the project's overview page. Here, you'll find a wealth of project-related information, including details on test cases, ongoing test runs, project activity, and more.

Should you wish to navigate to a different project at any point, simply return to the dashboard by clicking the link located in the upper left corner.

## Test Cases and Sections

A TestRail test case comprises a comprehensive description of test prerequisites, a sequence of test steps, and the anticipated outcome. Ideally, a single tester should be able to verify a test case in a relatively short time frame. Each test case serves the purpose of either confirming a specific functionality, documenting a task, or validating a project artifact.

Within the TestRail framework, test cases are efficiently organized into sections and subsections. These organizational units act as containers for test cases and are typically employed to categorize them based on specific project modules or product areas. The structuring of sections depends on the scope and complexity of your project. For projects with a substantial number of test cases within a module, it is advisable to further subdivide sections and create sub-sections to isolate distinct features or functionalities.

For instance, if you utilize multiple test cases to assess a particular application dialog or web page, these test cases should logically be grouped within a dedicated section for clarity and ease of management.

## Test Runs and Tests

To initiate a test and record the corresponding results for the test cases you've added, you commence a test run for a specific test suite. While a test suite functions akin to a blueprint detailing how an application is to be tested, a test run represents the actual execution of these tests in practice.

In most projects, you'll typically initiate multiple test runs for a particular test suite over time. For instance, in scenarios where you're releasing multiple versions of a software program, it's prudent to conduct a separate test run for each new release.

Moreover, it's entirely possible to have multiple concurrent test runs for a single test suite. This approach proves valuable when you need to execute the same test suite across various configurations, such as different operating systems. Consequently, you can commence a distinct test run for each unique configuration you intend to assess.

When initiating a new test run (e.g., by clicking the "Run a Test" button located in the test suite's toolbar), you have the flexibility to include all the cases from the test suite, select specific test cases, or employ dynamic filters based on specific test case attributes.

A test run comprises individual tests for each case you've incorporated. You can input test results and update the status of a test by either clicking the "Add Result" button on the test's page or making changes directly on the run's page.

The following test statuses are available by default:

- **Untested:** New tests start with the "Untested" status by default. Once a test result has been recorded, it cannot return to the "Untested" status.
- **Passed:** A test is marked as Passed when a tester verifies the test steps and the expected results.
- **Failed:** Testers designate a test as "Failed" if any of the specified test steps encounter errors or if the actual test result deviates from the expected outcome.
- **Retest:** If a developer or tester determines that a test needs to be reevaluated, they label it as "Retest." For instance, if a test initially failed and a developer subsequently rectified the issue, it can be marked for reevaluation.
- **Blocked:** The "Blocked" status is used when a test cannot be executed at present due to external dependencies, such as a bug that must be resolved before the test can be completed. This status is often employed in conjunction with the "Retest" status.

Once a test run reaches its conclusion, you can close it from the edit page of the run. Tests within a closed run become unmodifiable, which makes it an ideal choice for archiving purposes. Furthermore, any alterations made to the attributes of associated cases (such as the expected result) will not affect the closed and archived run.

## Projects and Their Types

Projects serve as the fundamental organizational cornerstone within TestRail. They serve as the primary container for all other data, including test runs, test results, milestones, and more, all of which are intricately linked to and attributed to a designated project.

## Milestones

In TestRail, you can include your project milestones in your workflow. These milestones can encompass significant project events, such as anticipated public software releases, internal test phases, or even specialized beta releases for key clients. Once you've integrated your milestones into TestRail, you gain the ability to allocate test runs to specific milestones.

This practice of assigning test runs to milestones offers several advantages. It enables you to conveniently monitor the progress and test results of each milestone individually. This proves especially valuable when you're concurrently working on multiple milestones or managing numerous active test runs. Effectively utilizing milestones within TestRail can greatly streamline your project management process.

## Test Plans and Configurations

When confronted with the task of managing multiple test runs and configurations within a single project, TestRail's test plans prove to be an invaluable tool. A test plan empowers you to initiate multiple test runs concurrently, particularly useful when assessing your project against various configurations. These configurations can encompass a range of elements, including different operating systems or web browsers.

To create a test plan, you can initiate the process by clicking the "Add Test Plan" button found on the "Test Runs & Results" page. Similar to configuring a single test run, you have the flexibility to define various properties of the test runs within the plan, such as their names, the specific cases to be included, and more.

Frequently, you'll encounter scenarios where you need to assess a particular test run against multiple configurations, such as various operating systems or web browser versions. Simplifying the creation of separate test runs for each configuration combination, TestRail allows you to specify and select all configurations for your test runs within a plan effortlessly. To achieve this, merely click the "Select Configurations" link associated with a run, and then proceed to select or add the desired configurations. This feature streamlines the process, enhancing efficiency in your testing efforts.

## Todos and Notifications

Tests within TestRail can be efficiently allocated to team members, offering flexibility in the assignment process. You can opt to assign tests either during the creation of a test run or at a later stage, directly from the run or test pages. Once a test has been designated to a specific user, it instantly becomes part of that user's todo list. Each user maintains an individual todo list for every project they are engaged in, while the Dashboard offers a convenient overview of all their pending tasks across various projects.

Moreover, the todo page provides the capability to not only view one's tasks but also those of fellow team members or the entire team simultaneously. This feature serves as a valuable resource for team leads, enabling them to efficiently delegate tests to team members with the lightest workload.

Additionally, TestRail offers email notifications as a pertinent feature. These notifications prove invaluable in keeping test owners informed about changes made by other users to their assigned tests. For instance, if a test is assigned to a user (i.e., the test owner), and another user adds a comment or records a test result for that test, the test owner receives prompt email notifications. Furthermore, users can choose to subscribe to tests owned by others or even entire test runs by simply clicking the small email icons available on the relevant pages. This functionality enhances communication and collaboration within the testing team, ensuring everyone stays informed and up-to-date.

# Tracking Progress and Activity

In addition to simplifying test case management and result entry, TestRail's capability to offer all team members a seamless means of monitoring test progress stands out as one of its most invaluable features. This feature allows you to effortlessly track the results and testing activity at the level of test runs, milestones, and entire projects via dedicated resource pages.

On the individual resource pages for test runs and milestones, you have the flexibility to choose from multiple viewing options. The sidebar provides convenient access to toggle between the status, activity, and progress views, enabling you to gain insights tailored to your specific needs and objectives.

Moreover, for a comprehensive overview at the project level, you can navigate between the project history and test results sections on the project's overview page. This allows you to delve into project-wide data effortlessly, making it easier to assess overall progress and performance.

For advanced reporting and more in-depth analysis, TestRail offers an array of additional reporting features accessible through the Reports tab. This resource-rich tab empowers you to generate and access insightful reports that provide a deeper understanding of your testing processes and outcomes.
