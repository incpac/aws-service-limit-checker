# AWS Service Limit Checker

This is a quick Python script that will get your current AWS Service Limits and compare them against the defaults.

## Example

```bash
$ get_service_quotas

+-------------------------------------------+-----------------------------------------------------+---------+---------+---------+
| service                                   | quota                                               | current | default | changed |
+===========================================+=====================+===============================+=========+=========+=========+
| AWS Cloud Map                             | DiscoverInstances operation per account burst rate  | 2000    | 2000    | False   |
+-------------------------------------------+-----------------------------------------------------+---------+---------+---------+
| AWS Cloud Map                             | DiscoverInstances operation per account steady rate | 1000    | 1000    | False   |
+-------------------------------------------+-----------------------------------------------------+---------+---------+---------+
| Amazon Elastic Compute Cloud (Amazon EC2) | All X Spot Instance Requests                        |    0    |    0    | False   |
+-------------------------------------------+-----------------------------------------------------+---------+---------+---------+
| Amazon Elastic Compute Cloud (Amazon EC2) | Running Dedicated a1 Hosts                          |    2    |    0    | True    |
+-------------------------------------------+-----------------------------------------------------+---------+---------+---------+
| Amazon Elastic Compute Cloud (Amazon EC2) | Running Dedicated c3 Hosts                          |    2    |    0    | True    |
+-------------------------------------------+-----------------------------------------------------+---------+---------+---------+
| Amazon Elastic Compute Cloud (Amazon EC2) | Running Dedicated c4 Hosts                          |    2    |    0    | True    |
+-------------------------------------------+-----------------------------------------------------+---------+---------+---------+
| Amazon Elastic Compute Cloud (Amazon EC2) | Running Dedicated c5 Hosts                          |    2    |    0    | True    |
+-------------------------------------------+-----------------------------------------------------+---------+---------+---------+
```
