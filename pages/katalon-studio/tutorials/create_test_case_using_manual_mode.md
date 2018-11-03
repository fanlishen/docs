Creating test case using manual mode
使用手动模式创建测试用例

预计阅读时间：3分钟

Katalon Studio supports Keywords-Driven testing where test cases consist of keywords that represent actions of users on the AUT (Applications Under Test). This allows users with less experience in programming to easily generate automation test. The below tutorial will give you step-by-step instruction in order to create an automation test case in manual mode.
Given a sample test case with the following steps:
*Open the browser
*Navigate to a website
*Click on a certain control
*Validate if the control exists on the page
*Close the browser

Katalon Studio支持关键字驱动测试，其中测试用例包含了用户在AUT(测试中应用程序）上所操作的关键字。这使得编程经验较少的用户可以轻松完成自动化测试。 以下教程将为您提供逐步说明，以便在手动模式下创建自动化测试用例。

以下是手动模式下示范测试用例步骤：

*打开浏览器
*导航到一个网站
*单击某个控件
*验证页面上是否存在控件
*关闭浏览器

Follow these steps to automate the above test scenario in Manual view:
按照以下步骤在**手动视图**中自动执行上述测试场景：

1.Select File > New > Test Case from the main menu to create a test case. .Provide the name for the new test case, then click OK.

1.从主菜单中选择File > New > Test Case创建测试用例，并输入新测试用例的名称，然后单击[ok]。


2. Once a new test case is created, it is opened in Manual view. This view allows users to define steps for the test case easily with little programming skills required.
2.创建新的测试用例后，将在[手动视图]中打开它。 此功能允许用户轻松创建测试用例，仅需要很少的编程技能。

3. Select Add > Web UI Keyword from the command toolbar.
3.从命令工具栏中选择  Add> Web UI keyword。

4. Select the Open Browser keyword. This keyword opens a browser and navigates to the specified URL if provided (the detail of a selected keyword is shown in the popup screen as shown below)
4 选择[open Browser]关键字。 如果提供url地址，该关键字将打开浏览器并导航到指定的URL（弹出悬浮窗中显示所选关键字的详细信息，如下图所示）


5. Add the Navigate To Url keyword. This keyword navigates to a specified URL. Double click on the Input cell to provide additional data (parameters) for the keyword.

5 添加[Navigate To Url]关键字。 此关键字导航到指定的URL。 双击[Input]单元格，为关键字提供其他数据（参数）。


6. The Input dialog is displayed as below. Each row represents one parameter.
6. [Input]对话框显示如下。 每一行代表一个参数。

详细信息：
名称    		描述
序列				该参数所选关键字进行排序
参数名称 		 参数的名称
参数类型 		 参数的类型（例如：字符串、变量或者测试数据值…）
值的类型 		 输入值的类型（例如：字符串、变量或者测试数据值…)
值					 此参数的输入值。输入值因指定的值类型而异。 有关详细信息，请参阅Katalon中的值类型。


For now, enter the URL of Katalon demo AUT (http://demoaut.katalon.com) into the Value column then click OK.

现在，在[value]列中输入Katalon示范的测试地址（http://demoaut.katalon.com），然后单击【ok】

7. Add the Click keyword. This keyword represents a click action on a given object. You need to associate this keyword to an object. Double click on the Object cell to open the Test Object Input dialog.
7.添加[Click]关键字。此关键字表示对给定对象进行单击操作。您需要将此关键字与对象关联。双击Object单元格以打开【Test Object Input】对话框。

8. All captured objects in Object Repository are displayed in the Test Object Input dialog (Refer to Spy Object for details regarding how to capture objects). Select your object then click OK.

8.「测试对象存储库」中的所有捕获对象都显示在「Test Obeject Input]对话框中（有关如何捕获对象的详细信息，请参阅[spy object]选择您的对象，然后单击Ok。

9. Add the Verify Element Present keyword. This keyword validates if a certain object is displayed on the executing browser. Similar to the previous step, you need to associate this keyword with an object.
9 .添加[Verify Element Present]关键字。此关键字验证在执行测试的浏览器上是否显示某个对象。与上一步类似，您需要将此关键字与对象关联。

10. Add the Close Browser keyword and save your test case.
10 .添加[Close Browser]关键字 将关闭并保存测试用例。


11. Click on Run in the main toolbar to execute the test case.
11 .单击主工具栏中的[Run ]以执行测试用例

Katalon Studio should be able to execute all of the steps specified in the test case. Test execution results are shown in Log Viewer as below:
Katalon Studio能够执行测试用例中指定的所有步骤。 测试执行结果显示在日志查看器中，如下所示：

