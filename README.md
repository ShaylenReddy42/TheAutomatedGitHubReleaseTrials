# The Automated GitHub Release Trials

## What's the purpose of this repo ?

To conduct trials using different Azure DevOps pipeline trigger rules to automate a GitHub Release

The result will be the strategy I will use for all my projects moving forward

This is a partial implementation of an AZ-400 exam objective

* Configure processes and communications (10-15%)
  * Configure collaboration and communication
    * configure release documentation, including release notes and API documentation

## Trials

### No. 1

Using the "tags" trigger rule and trigger on all tags

Expectations:

* Only if a tag is pushed to the repo, should it trigger. Any commits after, won't trigger it
* If it does trigger after a change, it means that the trigger rule will be met just because it forms part of a tag
* That behavior is not what I want

Results:

After a few attempts to get the pipeline definition right, the initial trigger rule I tried was the right one

Nuances:

* The initial GitHub service connection I had, didn't satisfy the task, so I had to create a new one
* I forgot to specify the pool
* And I incorrectly used a predefined variable, no idea how that happens

Well, that's it for these trials, didn't think I'd get on the first trigger rule because I misunderstood the definition of it in the docs and had a different idea in my other repo, "Seelan's Tyres" [here](https://github.com/ShaylenReddy42/Seelans-Tyres/commit/78dd7fea58e68b4452a54cdec0d434c4ff649524)