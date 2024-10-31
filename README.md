## 1. How scrapping done
     1- Download all necessary libraries such as requests, json, pandas etc
     2- Use Github API to fetch users with more than 100 followers
        'https://api.github.com/search/users?q=location:barcelona+followers:%3E100'
     3- For each user go to url users['url']
     4- get all the fields convert to pandas DF and convert to users.csv
     5. For each user in users.csv go to 'https://api.github.com'}/users/{user['login']}/repos?sort=pushed&direction=desc&page={page}&per_page=100'
     6- Take 500 recently pushed repositories and all the fields mentioned in the question
     7- convert to repositories.csv
## 2 Most interesting fact
  One intresting fact I learnt that even in the URL we can do filtering
  other intresting fact was that there is only 0.075 corellation between number of followers and the number of public repositories among users in
## An actionable recommendation for developers based on analysis
  No actionables

                         
