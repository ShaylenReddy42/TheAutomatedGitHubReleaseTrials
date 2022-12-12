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
