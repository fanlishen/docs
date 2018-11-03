使用脚本模式创建测试用例
预计阅读时间：4分钟

除了手动视图外，Katalon Studio还允许专家用户以编程方式在测试用例的脚本视图中编写自动化测试。具有Groovy / Java背景的用户可以在此视图中轻松编辑测试脚本。

本教程将指导您使用Katalon Studio手动编写非常基本的自动化测试脚本。阅读完本文后，您将能够理解并能够使用import语句和内置关键字来编写测试脚本。建议你应该有一些基本的脚本编写背景，最好使用Groovy，以有效地使用脚本功能。

给出一个带有以下步骤的示例测试用例：

打开浏览器
导航到一个网站
单击某个控件
验证页面上是否存在控件
关闭浏览器
按照以下步骤在脚本视图中自动执行上述测试方案：
1.从主菜单中选择 File > New > Test Case 以创建测试用例。提供新测试用例的名称，然后单击“OK”。

2.创建新的测试用例后，切换到“脚本”视图。手动视图中指定的测试步骤将自动转换为脚本视图中的Groovy脚本。

测试脚本中的import语句允许引用要使用的类。展开“import”部分以查看Katalon Studio的所有默认导入类。每个import语句中“as”后面的名称是该类的别名。您可以更改每个类的别名。这些类是编写测试脚本所必需的。

Katalon Studio是一款支持关键字驱动测试的自动化工具。所有关键字都相应地分为WebUI，Mobile和WebService包。按“Ctrl + Space”可从导入的类中查看这些包和函数。

3.在此测试方案中，您将创建Web应用程序测试脚本，以便可以使用Web UI内置关键字。要使用内置WebUI关键字，请在编辑器中输入以下语法。
WebUI.

4.输入点字符.之后，所有内置关键字及其对WebUI测试的描述如下所示

5.选择[Open Browser ]关键字。此关键字打开浏览器并导航到指定的URL（如果提供的话），所选关键字的详细信息显示在弹出屏幕中。

6.输入[Navigate To Url]关键字。此关键字导航到指定的URL。现在，输入www.katalon.com的网址作为参数的值。


7.输入Click.  此关键字表示对给定对象的单击操作。您需要为此操作指定一个对象。

8.使用以下语法可以引用Object Repository中的对象（或者，您可以将对象拖放到测试用例编辑器以生成语法）：

findTestObject（'{Object ID}'）

其中Object ID是Katalon Studio中该对象的ID值。

9.您可以从[Test Object Properties’对话框中找到对象的ID值。例如：

10.输入[Verify Element Present]关键字。此关键字验证在执行测试程序在浏览器上是否显示该对象。与上一步类似，您需要指定要与此关键字一起使用的对象。

11.添加[Close Browser]关键字并保存测试用例。

12.使用脚本时，以下API文档非常有用：

类			 			            描述
Builtin Keywords  			常见内置关键字列表
WebUI Builtin Keywords   		电脑端内置关键字列表
Web Service Builtin Keywords	接口内置关键字列表
Mobile Builtin Keywords		移动端内置关键字列表

13.恭喜！您已经使用Groovy语言完成了第一个自动化脚本。单击主工具栏中的“运行”以执行测试用例。


Katalon Studio应该能够执行测试用例的脚本。测试执行结果显示在日志查看器中，如下所示：
