## What is Code Review?
 When developers works  on creating new features or fixing bugs, they develop their changes on branches. In github, branches are separate “stages” where code is being developed without affecting  the code on other branches .
When a feature is completed, developer creates  Pull Request, where changes are requested to be merged to the main branch.
Finally, [Code Review](https://en.wikipedia.org/wiki/Code_review)  is the process performed during  pull request, where other developers check the code, add comments, and perform discussions with the developer about the proposed solution.

## How to Review the Code?
  Code review is a validation process that involves at least one reviewer other than the developer. When developer opens Pull Request, he/she select the reviewers and invite them for the discussion along with the other developers. 

Code review  allows developers to see a comparison between the original code and changes proposed by developer. Each line of code can be commented, as well as general comments can be added to Pull Request. Code review can end with three different outcomes:
* Accepted – when code is fine, and reviewer agrees to merge changes
* Rejected – where reviewer denies merging and requires changes to the proposed code.
* Comment – where a reviewer adds remarks but doesn’t make the decision about merging. It can be useful when PR is work-in-progress .

## What Do Code Reviewers Look For?
Code reviews should look at:

* <B>Design:</B> Is the code well-designed and appropriate?
* <B>Functionality:</B> Does the code behave as the developer likely intended?
* <B>Complexity:</B> Could the code be made simpler? Would another developer be able to easily understand and use this code when they come across it in the future?
* <B>Tests:</B> Does the code have correct and well-designed automated tests?
* <B>Naming:</B> Did the developer choose clear names for variables, classes, methods, etc.?
* <B>Comments:</B> Are the comments clear and useful?
* <B>Style:</B> Does the code follow our style guides?
* <B>Documentation:</B> Did the developer also update relevant documentation?

## The Goal of Code Review

* Improving code quality and reducing the number of bugs by sharing knowledge of developer and reviewers.
* The code review process enforces developers to follow certain coding practices throughout the  development phase. 
* Standardize the source code, making it convenient for all developers (even new ones) to study and understand it easily.
* Monitoring project quality and requirements


## Code Review Guidelines
* Make sure that there are no project Warnings/Errors.
* Perform Code Analysis on the project (with all Microsoft Rules enabled).
* <B>Code cleanup:</B> Remove all unused code.
      <br><B>Refer:</B>  http://msdn.microsoft.com/en-us/magazine/ee335722.aspx.</br>
* Perform 'null' checks wherever applicable to avoid the Null Reference Exception at runtime.
* Use related names or phrases to name a class so that developers can understand what the class consists of.
```csharp 
 public class IoTMessageNFT
   {
   }
public class ProtocolNFT
   {
   }
```
* Follow the define Naming Conventions (as recommended by Microsoft). 
                   <br> For variables/parameters, follow Camel casing </br>
                   <br> For method names and class names, follow Pascal casing </br>
     <br><B>Refer:</B> https://docs.microsoft.com/en-us/dotnet/standard/design-guidelines/capitalization-conventions?redirectedfrom=MSDN
* <B>Type Names</B> use predefined data type names instead of system data type names like Int32 etc.
* Avoid the use of underscore while naming identifiers.
```csharp
      //Correct 
    public double numberOfTransaction 
    public double totalBalance
    public double totalSpendableBalance

     //InCorrect
    public double number_Of_Transaction 
    public double total_Balance
    public double total_Spendable_Balance
```
* Always prefix an interface with letter I.
 ```csharp
   public interface INFT
    {
        string TypeText { get; set; }
        NFTTypes Type { get; set; }
        string Name { get; set; }
    } 
```
* Always declare the properties as private so as to achieve Encapsulation and ensure data hiding. 
* Constants should always be declared in UPPER_CASE.
* <B>Code Reusability:</B> Extract a method if the same piece of code is being used more than once or you expect it to be used in future. Make some generic methods for repetitive task and put them in a related class so that other developers start using them once you inform them. Develop common functionality so that they can be reused across the project.
   <br><B>Refer:</B> https://docs.microsoft.com/en-us/previous-versions/office/developer/office2000/aa140806(v=office.10)?redirectedfrom=MSDN
* <B>Code Consistency:</B> Maintain consistency for all data types across the application. For Example, if an Int32 type is coded as int and String type is coded as string, then they should be coded in that same fashion across the application. But not like sometimes int and sometimes as Int32.
* <B>Code Readability:</B> Should be maintained so that other developers understand your code easily
* Proper implementation of Exception Handling (try/catch and finally blocks) and logging of exceptions.
   <br><B>Refer:</B> https://docs.microsoft.com/en-us/previous-versions/dotnet/netframework-4.0/ms229005(v=vs.100)?redirectedfrom=MSDN
* Make sure that methods have less number of lines of code. Not more than 30 to 40 lines.
* Write comments on top of all methods to describe their usage and expect input types and return type information.
    ```csharp
   /// <summary>
        /// Create short version of address, 3 chars on start...3 chars on end
        /// </summary>
        /// <param name="address"></param>
        /// <returns></returns>
        public static string ShortenAddress(string address)
        {
            if (string.IsNullOrEmpty(address))
                return string.Empty;
            var shortaddress = address.Substring(0, 3) + "..." + address.Substring(address.Length - 3);
            return shortaddress;
        }
   ```
* Timely check-in/check-out of files/pages at source control.
* <B>Unit Testing:</B> Write test cases and perform unit testing to make sure that basic level of testing is done before it goes to QA testing
     <br><B>Refer:</B> https://docs.microsoft.com/en-us/previous-versions/visualstudio/visual-studio-2015/test/unit-test-basics?view=vs-2015&redirectedfrom=MSDN
* Use constants and readonly (modifier) wherever applicable.
* Try using LINQ queries and Lambda expressions to improve Readability
     <br><B>Refer:</B> https://docs.microsoft.com/en-us/previous-versions/dotnet/articles/bb308959(v=msdn.10)?redirectedfrom=MSDN
* Use access specifiers (private, public, protected) as per the scope of methods, classes, or  variables.
