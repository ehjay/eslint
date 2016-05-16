# Rule Deprecation

Balancing the trade-offs of improving a tool and the frustration these changes can cause is a difficult task. One key area in which this affects our users is in the removal of rules.

The ESLint team is committed to making upgrading as easy and painless as possible. To that end, the team has agreed upon some guidelines for deprecating rules in the future. The goal of these guidelines is to allow for improvements and changes to be made without breaking existing configurations.

Until May 1, 2017, the team has committed to not remove any rules in any releases of ESLint; however, the team will deprecate rules as needed. When a rule is deprecated, it means that:

* The team will no longer do any work on the rule. This includes bug fixes, enhancements, and updates to the rule's documentation. Issues and pull requests related to the deprecated rule will not be accepted and will be closed automatically.
* The rule is moved to a list of deprecated rules rather than being on the main rule page. Additionally, the rule will be labeled as deprecated on the rule's documentation page.

After May 1, 2017, the team will revisit all deprecated rules and evaluate whether they should actually be removed or not. If the rule is removed at this time, users will have to adjust their configuration accordingly.

We hope that by following these guidelines we will be able to continue improving and working to make ESLint the best tool it can be while causing as little disruption to our users as possible during the process.
