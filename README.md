Service Status
===============
Please [follow us on Twitter](https://twitter.com/BeShippable) for latest service status updates, important changes, and new feature announcements.

Known Issues
===============
**SSH Keys Reset due to a bug:** There was a bug introduced on 11 Aug 2015 that caused the subscription SSH keys used for deployment and encryption to be reset.    

***Impact:***     
1. All projects that required Shippable to be authenticated by any provider during any part of the build workflow will need to reset their Shippable SSH keys at the provider.     
2. If you are using encrypted variables, this will also break since we use the SSH keys to encrypt. You will need to re-encrypt the keys and update the YML.   

***How to fix:*** Go to your Subscription -> Settings. Copy the Deployment Key there and use that in the appropriate section within your provider account. For instance, if you are using Github and have multiple projects in Shippable, you will need to reset the SSH keys under your Profile->Settings. 

Please contact us at support@shippable.com if you have any ```Authentication or Permission Denied``` errors in your builds and the solution above does not work. Our sincere apologies for the inconvenience.

Shippable Support
=================

This repository tracks [bugs and feature requests] (https://github.com/Shippable/support/issues?state=open) for Shippable's docker based continuous integration and deployment platform.

If you are seeing issues pulling or pushing to docker hub, please check if docker hub is experiencing problems before opening a support issue - https://status.docker.com/pages/history/533c6539221ae15e3f000031

Create New Issue 
------------

* Go to the [issues list] (https://github.com/Shippable/support/issues?state=open) and create a new issue
* Please try to describe the issue with as many screenshots and details as possible
* For bugs, don't forget to include - github/bitbucket username of the account which enabled the repository, and shippable.yml + any scripts called from the yml.
* If your issue is about a build failure, please include a link to a failed build.


Track Issue Status 
------------

**We will triage issues within 24 hours.** We will update the issue frequently with latest status, so you will be constantly aware of what is happening.  Please note if you have a blocking issue -- we can escalate resolution priority. 

We will update the issue with these tags as the bug goes through our process -
* [triaged] (https://github.com/Shippable/support/issues?labels=triaged&page=1&state=open) after we have looked at the bug and decided on a course of action.
* [in progress] (https://github.com/Shippable/support/issues?labels=in+progress&page=1&state=open) when it is actually assigned to an engineer. 
* [deployed] (https://github.com/Shippable/support/issues?labels=deployed&page=1&state=open) when code changes are complete and deployed into production.

Feel free to [open your issue now] (https://github.com/Shippable/support/issues?state=open)!
