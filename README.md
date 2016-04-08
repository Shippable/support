Shippable Support
=================

This repository tracks [bugs and feature requests] (https://github.com/Shippable/support/issues?state=open) for Shippable's docker based continuous integration and deployment platform.

Before opening a new Support Issue:
-----------------------------------

* Please [follow us on Twitter](https://twitter.com/BeShippable) for latest service updates, important changes, and new feature announcements.
* If you are seeing issues pulling or pushing to docker hub, please check if [docker hub is experiencing problems](https://status.docker.com/pages/history/533c6539221ae15e3f000031) before opening a support issue.
* Known issues:

  - Builds fail with `alerts/errors/failed to find yml file`, a `shippable.yml` needs to be created. An example for [reference](http://docs.shippable.com/ci_configure/#shippableyml-structure).
  - Builds fail with `alerts/errors/invalid yml format`, validate your `shippable.yml` using [YAML Lint] (http://www.yamllint.com/) or [YAML Online Parser](http://yaml-online-parser.appspot.com/).
  - Builds fail with `git_sync\Host verification key failed`, refer to [Tip 5 for a successful migration](http://blog.shippable.com/5-tips-for-a-successful-migration).

Open a new Support Issue:
-------------------------

* Go to the [issues list] (https://github.com/Shippable/support/issues?state=open) and create a new issue.
* The following is needed to expedite the resolution of your issue:

    - Describe the issue with as many details as possible.
    - If your issue is regarding a **build failure**, it is essential to include:

        - Link to the failed build. The URL of the failed build includes the buildID needed for troubleshooting
        - `shippable.yml`
        - Any scripts called from the yml
    - Indicate if the issue is impacting your business and/or is blocking
* NOTE: the absence of the above information will delay the mitigation of the issue

Track Issue Status:
------------------

**We triage all new issues in 1 business day.** We will update the issue frequently with latest status, for you to be up to speed on the progress towards resolution.

NOTE: If you have an issue that is impacting your business and/or is blocking, please indicate it in your support issue. We will escalate and prioritize resolution.

Support Process:
----------------
During the triage, we tag the support issues per our Support Process flow.

**Process related labels:**

- [investigate](https://github.com/Shippable/support/labels/investigate): The issue is being investigated by Shippable engineers, including reproducing the issue to determine if it is a bug or feasibility if it is a feature request.
- [implement](https://github.com/Shippable/support/labels/implement): The issue has gone through Shippable’s daily internal support triage and the next step toward resolution has been initiated.
- [in progress](https://github.com/Shippable/support/labels/in%20progress): The identified resolution is in the process of being designed, developed, tested & deployed.
- [need info from customer](https://github.com/Shippable/support/labels/need%20info%20from%20customer): Shippable requires additional information regarding the issue in order to continue troubleshooting the issue. The customer who opened the issue is accountable to provide this information, to make progress towards resolution.
- [resolved](https://github.com/Shippable/support/labels/resolved): The issue has been mitigated either through code changes deployed into production and/or the issue has been successfully addressed.

The issue will be closed if it meets one of the following conditions:

- The issue has been tagged **resolved** and 5 business days have passed with no confirmation from the customer.
- The issue has been tagged **need info from customer** and 7 business days have passed with no response from the customer.
- The issue has been tagged **duplicate** and has the link to the original issue being tracked.

The above process/tags are transparent, thereby enabling our customers who opened support issues to know the most current status of their issues.

**Issue related labels:**

- [bug](https://github.com/Shippable/support/labels/bug): Shippable has determined that the product is not behaving the way it is intended to. It requires a code change to resolve the issue.
- [feature request](https://github.com/Shippable/support/labels/feature%20request): Feature currently does not exist. If implemented, it is intended to provide additional value to our customers
- [update content](https://github.com/Shippable/support/labels/update%20content): Customer specifically wants to know how to use/implement a feature. Issues tagged so will be updated in one of our content platforms such as Documentation, Blogs, videos for customers to self-serve in the future.
- [technical issue](https://github.com/Shippable/support/labels/technical%20issue):  Customer is unable to use Shippable service per expectation & needs help to resolve the issue. Issues determined to be bugs & feature requests will not be tagged as technical issues.
- [duplicate](https://github.com/Shippable/support/labels/duplicate): This exact issue is already being tracked

There are other labels, not documented here, that Shippable uses internally for classifying and assigning the support tickets.
