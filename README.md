# WBT-frontend-task-2

This task tests your proficiency in working with REST API and React Frameworks. You'll using the Github api for this task.

In this Task:
* List the most starred Github repos that were created in the last 30 days.
* Show the result as a list. One repository per row.
* Show the Following fields in your display: 
  * Repository name,
  * Repository description.
  * Number of stars for the repo.
  * Number of issues for the repo.
  * Username and avatar of the repo owner.
* Implement data pagination with infinite scroll.(optional)

## Using Github search API

To get the most starred Github repos created in the last 30 days (relative to 2021-09-13), you'll need to call the following endpoint : 
`https://api.github.com/search/repositories?q=created:>2021-08-13&sort=stars&order=desc`

The JSON data from Github will be paginated (you'll receive around 100 repos per JSON page). 

To get the 2nd page, you add `&page=2` to the end of your API request : 

Read more about the Github API over [here](https://developer.github.com/v3/search/#search-repositories
).

## Mockups
![alt text](https://raw.githubusercontent.com/hiddenfounders/frontend-coding-challenge/master/mockup.png)

Here's what each element represents :

![alt text](https://raw.githubusercontent.com/hiddenfounders/frontend-coding-challenge/master/row_explained.png)
