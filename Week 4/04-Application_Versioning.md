# Application Versioning
Application versioning in Pega refers to the process of managing and tracking different versions of a Pega application as it evolves over time. Versioning allows developers to maintain a history of changes, control deployments across different environments, and ensure consistency and integrity of the application's configuration. 

## Lock and Roll
Small changes or patches are ideal for lock and roll. Application patches and minor updates usually involve updating rules. When using lock and roll, you create a new empty ruleset version. To update the configuration, you copy the necessary rules into the new ruleset version.

The rule in the higher ruleset version overrides the rule in the lower version. You specify the new version number and whether to update the application record and access groups to reflect the ruleset version.


## Skimming
Skimming is the process of saving the highest version of a rule into a new, higher ruleset version. Skimming applies mainly to resolved rules. Skimming is useful when rule changes follow a logical sequence. The two types of skims are minor and major. The skim types correspond with the update types (major or minor/patch).

During a minor skim, rules are stored in a higher minor version, and during a major skim, rules are stored in a higher major version.

A rule's availability status determines if the rule is carried forward. This table defines the rules that are carried forward during a skim.
<table border="1">
  <tr>
    <th>Rule Availability Status</th>
    <th>Carried forward?</th>
  </tr>
  <tr>
    <td>Available</td>
    <td>Yes</td>
  </tr>
  <tr>
    <td>Blocked</td>
    <td>Yes</td>
  </tr>
  <tr>
    <td>Final</td>
    <td>Yes</td>
  </tr>
  <tr>
    <td>Withdrawn</td>
    <td>No - major update; Yes - minor update</td>
  </tr>
  <tr>
    <td>Not Available</td>
    <td>No</td>
  </tr>
</table>
