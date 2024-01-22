# github-workflow

#### To search for all the events for github we can visit
[Workflows](https://docs.github.com/en/actions/using-workflows/events-that-trigger-workflows)


## Events
1. we can add a single event ```on:push```
2. If we have multiple events then we can wrap in ```on:[push, workflow_dispatch]```

## Actions (specfic to github)
1.  they provide common used set instruction which we run on the target servers like pull code from repo.
2.  We either create our own actions or use actions from the marketplace [marketplace](https://github.com/marketplace?type=).
3. commonly used action [checkout_action](https://github.com/marketplace/actions/checkout)
4. sometime these commonly used action have certain configuration that are mentioned in docs and are done
using ```with:``` keyword

5. for runner machines we can check using [runner]()


## Running jobs in series
1. add ```needs: test``` property below the a jobs and the jobs name that needs to be completed before starting the current one
2. if have multiple jobs then ```needs:[job1, job2]```

## Experssion and Context Objects
1. to access environment variables and other things we can use expression and context objects
2. list of all the context objects are available on [link](https://docs.github.com/en/actions/learn-github-actions/contexts)

## Event Activity Type and Filters
1. Some events have activity type for `pull_request: opened`
2. Filter control when will the event will be triggered `push Event : filter based on a branch`