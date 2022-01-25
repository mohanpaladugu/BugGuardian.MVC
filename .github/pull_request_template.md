## What is a Pull Request?

A pull request (sometimes called merge requests) is a review request, is done by someone in the team to check the changes on a branch before merging into another branch.
<br>The changes being proposed could be either minor or major changes to the project. When a pull request is initiated, developers or maintainers of the project are able to review the proposed changes, suggest edits, and approve the proposed changes to be merged.</br>


## Why Use Pull Requests?
* to check whether [coding guidelines](https://github.com/fyziktom/VirtualEconomyFramework/wiki/Code-Review-Guidelines)  are followed.
* to check the code is tested thoroughly and has no issues.
* to check if code addresses given requirements
* to educate other team members about the changes made.

## Merge/Pull Request guidelines

* If you are a contributor, 
               <p>&emsp; please fork the repository you would like to contribute to.</p> 
               <p>&emsp;See the GitHub documentation for [forking a repo](https://docs.github.com/en/get-started/quickstart/fork-a-repo)</p> 
 If your developer/Maintainer you can clone the repository to your local workspace.

* Make sure that changes follow the  coding guidelines, completes the build successfully and passes all tests.

* while commiting the changes follow the commit messages guidelines.
      <br><B>Refer:</B>https://docs.gitlab.com/ee/development/contributing/merge_request_workflow.html#commit-messages-guidelines</br>
      <br><B>Refer:</B>https://cbea.ms/git-commit/</br>

* Pull requests should be created when you merge the changes to develop/master branch. Always get the latest version from the source branch before merging.

* while creating the PR it should refer to the Zen Hub ticket it is addressing. 
  <br>It should defined in the form {Story/Bug number}-{Project Name} tag as the first part of the title where {Story/Bug number}is the Zen Hub ticket number and {Project Name} in the Zen Hub .</br> 
Example: VEFramework-11. The ticket number should be part of the title not the PR body.

* Include a title that provides a one sentence overview of the purpose of the PR. 

* Description should contain complete information of the changes being made .

* Each contributor may only create one pull request at a time. Once your pull request has been merged, you can create another one. 

*  If the pull request has issues, or would require a significant rewrite to be acceptable, request will be rejected.

*  All pull request must have test units. if  for any reason, the tests are not added, please explain the reason. In that case, explained the steps followed to test your changes.

*   Maintainers/ contributors/Developers can participate in reviewing pull-requests

* An approval required from at least one approvers before changes can be merged.
