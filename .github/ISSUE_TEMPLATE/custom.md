---
name: Custom issue template
about: Describe this issue template's purpose here.
title: ''
labels: ''
assignees: ''

---

## What is Issue?
A project issue is a problem that has been encountered in executing project activities. 

Project's responsibility is to ensure that the tasks/features work the way they should and if they fails to meet the result, it becomes an Issue or Defect that need to be fixed.

## The Type Of Issues
Issues can be classified as below based on the nature it occurs on.

* <B>Functionality:</B> A functionality Issue is raised when a product does not work as expected.
* <B>Performance:</B> A performance Issue is raised when a product fails to meet performance considerations such as load time, speed and so on.
* <B>UI/UX:</B> An Issue becomes a UI/UX type when the product fails to meet the front end design standards in terms of theme, neatness, usability, and so on.
* <B>Compatibility:</B> This type of Issue implies that they don’t fit well across devices and screen dimensions.
* <B>Security:</B> Any issues related to application security. Example: SQL injections, vulnerabilities, buffer overflows, weak authentication,DoS

## Prioritize Issues
Priority defines the order in which the issues will be addressed or resolved.  Below are the Priority types:

* <B>Low:</B> The Issue can be worked upon even later on.
* <B>Medium:</B> The Issue deserves attention but not immediate.
* <B>High:</B> The Issue deserves attention and needs to be fixed as soon as possible.
* <B>Show Stopper:</B> The Issue needs to be prioritized and fixed immediately before anything else.

## Issues Severity
  Issue severity is defines based on the business impact of the task. Below are the Severity types:

* <B>Minor:</B> The Issue has very less impact on the project.
* <B>Major:</B> The Issue will have a considerable impact on the project.
* <B>Critical:</B> The Issue has a tremendous impact on the project.
* <B>Blocker:</B> The Issue acts as a show stopper for the project. The project cannot proceed further without resolving this Issue.

## Monitor Issue Resolution Status

Issue resolution status reflects the current state of the given issue. Below are stages of the issue.

* <B> New:</B> The Issue has been created and needs to be assigned.
* <B> Assigned:</B> The Issue has been assigned to be fixed by a developer.
* <B> InProgress</B>​ the issue is being worked on(work-in-progress)
* <B> Reopen:</B> The Issue has been marked resolved by a developer but hasn’t been completely corrected.
* <B> test:</B> The Issue has been fixed and is being tested.
* <B>Fixed:</B>The Issue has been resolved and marked Fixed by the developer.
* <B>Closed:</B> The Issue has been verified as resolved and closed by the tester.
![](https://ipfs.infura.io/ipfs/QmTbZaVMotBVovqy4xzSgc8U2CYyaDcwyjkL6JYvj6wiui)

## The industry standard naming convention

The proposed formats for <B>user story titles</B> are:
```
* As <a> <person/type of user>, I want <something> so that <some reason> 
   (e.g. As Sam Spends a lot, I want to one-click purchase so that I can get my goods as quickly as possible)
* As a <person/type of user>, I want <something> 
   (e.g. As a User, I want to create a task)
* <person/type of user> <performs action on> <thing> 
   (e.g. User visits home page OR User creates a task)
```

The proposed formats for bug titles are:
```
* <person/type of user> can’t <perform action/get result they should be able to> 
(e.g. New User can’t view home screen).
*  When <performing some action/event occurs>, the <name of the feature name> doesn’t work
* <system feature> doesn’t work
*  <system feature> should <expected behavior> but doesn’t
*  <system feature> <is not/does not> <expected behavior>
*  <persona/user type> <gets result> but should <get different result>
*  <quick name>. <one of the formats above> 
(e.g. “Broken button. New User can’t click the Next button on Step 2 of the Wizard”).
```

The proposed title formats for new features are:
```
Implement <endpoint> (e.g. Implement POST /api/v1/users)
Create endpoint <endpoint> (e.g. Create endpoint POST /api/v1/users)
```


The proposed title formats for improvements are:
```
* <endpoint> > also <additional functionality> (e.g. POST /api/v1/users > also accept date of birth)
* Make <feature> run faster
* Improve the performance of <feature/screen/endpoint>
* Update <feature> <with/to> <update>
* Rename <feature/text> to <new name>
```

Create an issue by clicking on New issue button
![](https://ipfs.infura.io/ipfs/QmVSFKKRyQ6NT53xTsT4765ykbsw6dPY7qHX1bLp7rMsTU)
 
Follow standard naming convention and clearly describe the issue in write section while creating the issue
![](https://ipfs.infura.io/ipfs/QmVqnQBJfm5LtiitEAYUCpomki9RMg7i63EFosE59PZj25)</br>

Label the issue as bug.

![](https://ipfs.infura.io/ipfs/QmbawiD9EJ8XZfv2VPjcdMAv5W3PM86vf1kQagHVvDA2CR)


After fixing the bug if application working as expected. Then we will close the issue with proper comments.
![](https://ipfs.infura.io/ipfs/QmaUpdKbRRCrYGiH8PT15HEtsHT7ttqVgJZj2ZptEUHCXC)

![](https://ipfs.infura.io/ipfs/QmTCf7g2BvuJfxGupiZKGDZiNknh1wj23renkcGm6uVvVQ)

## Issue guidelines:

* Don't raise two issues in one issue ticket. Open separate ticket for each issue.
* Don’t work on multiple issues in the same branch. If a feature is dropped, it will be difficult to revert changes.
* Always create one pull request addressing one issue. Don't create one pull request addressing multiple issues.
* Allocate deadlines for closing an issue and track the duration between opening and closing the issue.
* use Zen HUB for communicating defects with team members.
* Fix an appropriate basis for categorizing Issues based on specifics such as priority, severity and so on
* Assigning responsibility to team members for fixing the Issues.
* Create a screen shot highlighting the section where the issue can be see and upload in to issue tracking tool (Zen Hub)
