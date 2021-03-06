# Module 3: Introduction to JavaScript

# Lesson 3: Introduction to jQuery

### Demonstration: Adding jQuery to a Web Project

#### Preparation Steps 

1. Ensure that you have cloned the 20480C directory from GitHub. It contains the code segments for this course's labs and demos. https://github.com/MicrosoftLearning/20480-Programming-in-HTML5-with-JavaScript-and-CSS3/tree/get_started/Allfiles.

#### Demonstration Steps

#### Add jQuery to a project by using nuGet

1.	On the Windows 10 **Start** screen, click the **Visual Studio 2017** tile.
2.	In Visual Studio, on the **File** menu, point to **New** and then click **Web Site**.
3.	In the **New Web Site** dialog box, in the middle pane click **ASP.NET Empty Web Site**.

>**Note:** It does not matter whether you select the **Visual Basic** or **Visual C#** templates in the left pane; the templates for both languages enable you to create HTML5 web pages and implement functionality by using JavaScript.

4.	From the **Web location** list, click **File System**, set the file path to **Allfiles\Mod03\Democode\jQueryDemoTest**, and then click **OK**.
5.	On the **Tools** menu, point to **Library Package Manager**, and then click **Manage NuGet Packages for Solution**.
6.	In the **Manage NuGet Packages** dialog box, click **Online**. A list of available packages for download appears in order of popularity.
7.	In the **Search Online** box, type **jQuery**.
8.	In the list of packages, click **jQuery**, and click **Install**.
9.	In the **Select Projects** dialog box, click **OK**.
10.	In the **Manage NuGet Packages** dialog box, click **Close**.
11.	In Solution Explorer, notice that a **Scripts** folder has been added to the project and that it contains three files.

>**Note:** The three files are the uncompressed jQuery library, a minified version for use on production servers, and an IntelliSense file for Visual Studio to use.

12.	On the **File** menu, click **Save jQueryDemoTest**.

#### Enable jQuery IntelliSense

1.	In the Solution Explorer window, right-click the **Scripts** folder, point to **Add**, and then click **JavaScript File**.
2.	In the **Specify Name for Item** dialog box, type **test**, and then click **OK**.
3.	Type the following code and notice that IntelliSense is unable to offer suggestions for statement completion for jQuery functions such as **ready**.
    ```javascript
        $(document).ready(function () {
            // your code here
        });
    ```
4.	In the Solution Explorer window, right-click the **Scripts** folder, point to **Add**, and then click **JavaScript File**.
5.	In the **Specify Name for Item** dialog box, type **_references.js**, and then click **OK**.
6.	Add the following code to _references.js and then save it.
    ```javascript
        /// <reference path="jquery-1.8.2.js" />
    ```
>**Note:** If necessary, replace the jQuery version number (1.8.2) with that of the files downloaded by the package manager.

7.	In the _references.js file, type the following code and notice that IntelliSense is now able to offer suggestions for statement completion for jQuery functions, including the **ready** function.
    ```javascript
        $(document).ready(function () {
            // your code here
        });
    ```
8.	On the **File** menu, click **Save All**.
9.	Close Visual Studio 2017.

### Demonstration: Displaying Data and Handling Events by Using JavaScript

#### Preparation Steps 

1. Ensure that you have cloned the 20480C directory from GitHub. It contains the code segments for this course's labs and demos. https://github.com/MicrosoftLearning/20480-Programming-in-HTML5-with-JavaScript-and-CSS3/tree/get_started/Allfiles.

©2018 Microsoft Corporation. All rights reserved.

The text in this document is available under the  [Creative Commons Attribution 3.0 License](https://creativecommons.org/licenses/by/3.0/legalcode), additional terms may apply. All other content contained in this document (including, without limitation, trademarks, logos, images, etc.) are  **not**  included within the Creative Commons license grant. This document does not provide you with any legal rights to any intellectual property in any Microsoft product. You may copy and use this document for your internal, reference purposes.

This document is provided &quot;as-is.&quot; Information and views expressed in this document, including URL and other Internet Web site references, may change without notice. You bear the risk of using it. Some examples are for illustration only and are fictitious. No real association is intended or inferred. Microsoft makes no warranties, express or implied, with respect to the information provided here.
