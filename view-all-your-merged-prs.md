I have an accomplishments document that's shared with my manager where I keep updates on work I've done over the fiscal year. My goal is to update this monthly but that doesn't always happen. The most annoying part of this is linking each work item to a PR on GitHub. I've put together a saved search in GH to help and it looks like this:

`org:[yourOrg] is:pr author:[yourUsername] create:[dateRange] is:merged`

Example:
`org:heroku is:pr author:sarassassin created:>2022-01-31  is:merged`


Here's a bonus search snippet I use to view PR's opened by my teammates that need review:

`is:open is:pr team-review-requested:heroku/front-end -draft:true -label:"in progress" -label:dependencies NOT snyk in:title `


Drop these in the [GitHub Pulls query](https://github.com/pulls) or [Advanced Search](https://github.com/search) and have fun.
