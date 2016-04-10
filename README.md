Shippable Support
=================

This repository tracks [bugs and feature requests] (https://github.com/Shippable/support/issues?state=open) for Shippable's docker based continuous integration and deployment platform.

Before opening a new Support Issue:
-----------------------------------

* Please [follow us on Twitter](https://twitter.com/BeShippable) for latest service updates, important changes, and new feature announcements.
* If you are seeing issues pulling or pushing to docker hub, please check if [docker hub is experiencing problems](https://status.docker.com/pages/history/533c6539221ae15e3f000031) before opening a support issue.
* Known issues:

  - Documented [CI FAQs](http://docs.shippable.com/ci_faq/) and [Pipelines FAQs](http://docs.shippable.com/pipelines_faq/).
  - Create a `shippable.yml` for the error shown below. An example for [reference](http://docs.shippable.com/ci_configure/#shippableyml-structure).

<img src="../images/error_missing_yml.png" alt="Missing yml" style="width:700px;"/>

  - Validate your `shippable.yml` using [YAML Lint] (http://www.yamllint.com/) or [YAML Online Parser](http://yaml-online-parser.appspot.com/) for the error shown below.

<img src="../images/error_bad_yml.png" alt="Bad yml" style="width:700px;"/>

  - Refer to [Tip 5 for a successful migration](http://blog.shippable.com/5-tips-for-a-successful-migration) for the error shown below.

<img src="../images/error_hostkey_verification.png" alt="Hostkey Verification" style="width:700px;"/>

Open a new Support Issue:
-------------------------

* Go to the [issues list] (https://github.com/Shippable/support/issues?state=open) and create a new issue by filling out the New Issue Template.
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

-  [investigate](https://github.com/Shippable/support/labels/investigate)/[implement](https://github.com/Shippable/support/labels/implement): The issue has gone through Shippable’s daily internal support triage and the next action towards resolution has been identified and initiated.
- [in progress](https://github.com/Shippable/support/labels/in%20progress): An engineer is actively working on resolving the issue.
- [need info from customer](https://github.com/Shippable/support/labels/need%20info%20from%20customer): Shippable requires additional information regarding the issue in order to continue troubleshooting the issue. The customer who opened the issue is accountable to provide this information, to make progress towards resolution.
- [resolved](https://github.com/Shippable/support/labels/resolved): The issue has been mitigated either through code changes deployed into production and/or the issue has been successfully addressed.
- [deferred](https://github.com/Shippable/support/labels/deferred): The resolution of this issue has been deferred for now and will not be actively worked on.

The issue will be closed if it meets one of the following conditions:

- The issue has been tagged **resolved**. Customers are welcome to re-open the issue if they feel their issues are not resolved.
- The issue has been tagged **need info from customer** and 3 business days have passed with no response from the customer.
- The issue has been tagged **duplicate** and has the link to the original issue being tracked.
- The issue has been tagged **deferred**.

The above process/tags are transparent, thereby enabling our customers who opened support issues to know the most current status of their issues.

**Issue related labels:**

- [bug](https://github.com/Shippable/support/labels/bug): Shippable has determined that the product is not behaving the way it is intended to. It requires a code change to resolve the issue.
- [feature request](https://github.com/Shippable/support/labels/feature%20request): Feature currently does not exist. If implemented, it is intended to provide additional value to our customers
- [update content](https://github.com/Shippable/support/labels/update%20content): Customer specifically wants to know how to use/implement a feature. Issues tagged as such, will be updated in one of our content platforms such as Documentation, Blogs, videos for customers to self-serve in the future.
- [technical issue](https://github.com/Shippable/support/labels/technical%20issue):  Customer is unable to use Shippable service per expectation & needs help to resolve the issue. Issues determined to be bugs & feature requests will not be tagged as technical issues.
- [question](https://github.com/Shippable/support/labels/question): All non-technical issues faced by customers. For e.g. billing questions.
- [duplicate](https://github.com/Shippable/support/labels/duplicate): This exact issue is already being tracked

There are other labels, not documented here, that Shippable uses internally for classifying and assigning the support tickets.
