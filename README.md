# Awesome Cloud Security [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
> Cloud Security blogs, podcasts, standards, projects, and examples.
## Contents
* [Public Cloud Governance](#public-cloud-governance)
  * [AWS Governance](#aws-governance)
  * [MultiCloud Governance](#multicloud-governance)
  * [AWS - Patterns](#aws---patterns)
  *  [URL Services](#url-services)
* [Containers](#containers)
  * [Docker Images](#docker-images)
  * [Kubernetes Operators](#kubernetes-operators)
  * [Container Tools](#container-tools)
* [Cloud Security Standards](#cloud-security-standards)
* [Learning](#learning)
  * [Blogs](#blogs)
  * [Courses](#courses)
  * [Labs](#labs)
  * [Podcasts](#podcasts)
  * [Vulnerable by Design](#vulnerable-by-design)
* [Certifications](#certifications)
* [Projects](#projects)
  * [Alerting](#alerting)
  * [Benchmarking](#benchmarking)
  * [Data Loss Prevention](#data-loss-prevention)
  * [Identity and Access Management](#identity-and-access-management)
  * [Incident Response](#incident-response)
  * [Spring](#spring)
* [Examples](#examples)
  * [Automated Security Assessment](#ex-automated-security-assessment)
  * [Identity and Access Management](#ex-identity-and-access-management)
  * [Logging](#ex-logging)
* [Misc](#misc)
  * [Other Awesome Lists](#other-awesome-lists)
* [Contribute](#contribute)
* [License](#license)
## Public Cloud Governance
### AWS Governance
* [AWS CloudFormation Guard](https://github.com/aws-cloudformation/cloudformation-guard)
* [AWS CodePipeline Governance](https://github.com/awslabs/aws-codepipeline-governance)
* [AWS Config Rules Development Kit](https://github.com/awslabs/aws-config-rdklib)
* [AWS Control Tower Customizations](https://github.com/awslabs/aws-control-tower-customizations)
* [AWS Security Hub Automated Response and Remediation](https://github.com/awslabs/aws-security-hub-automated-response-and-remediation)
* [AWS Vault](https://github.com/99designs/aws-vault)
* [AWS Well Architected Labs](https://github.com/awslabs/aws-well-architected-labs)

* ## AWS - Patterns

### URL Services

| Service      | URL                   |
|--------------|-----------------------|
| s3           | https://{user_provided}.s3.amazonaws.com |
| cloudfront   | https://{random_id}.cloudfront.net |
| ec2          | ec2-{ip-seperated}.compute-1.amazonaws.com |
| es           | https://{user_provided}-{random_id}.{region}.es.amazonaws.com |
| elb          | http://{user_provided}-{random_id}.{region}.elb.amazonaws.com:80/443 |
| elbv2        | https://{user_provided}-{random_id}.{region}.elb.amazonaws.com |
| rds          | mysql://{user_provided}.{random_id}.{region}.rds.amazonaws.com:3306 |
| rds          | postgres://{user_provided}.{random_id}.{region}.rds.amazonaws.com:5432 |
| route 53     | {user_provided} |
| execute-api  | https://{random_id}.execute-api.{region}.amazonaws.com/{user_provided} |
| cloudsearch  | https://doc-{user_provided}-{random_id}.{region}.cloudsearch.amazonaws.com |
| transfer     | sftp://s-{random_id}.server.transfer.{region}.amazonaws.com |
| iot          | mqtt://{random_id}.iot.{region}.amazonaws.com:8883 |
| iot          | https://{random_id}.iot.{region}.amazonaws.com:8443 |
| iot          | https://{random_id}.iot.{region}.amazonaws.com:443 |
| mq           | https://b-{random_id}-{1,2}.mq.{region}.amazonaws.com:8162 |
| mq           | ssl://b-{random_id}-{1,2}.mq.{region}.amazonaws.com:61617 |
| kafka        | b-{1,2,3,4}.{user_provided}.{random_id}.c{1,2}.kafka.{region}.amazonaws.com |
| kafka        | {user_provided}.{random_id}.c{1,2}.kafka.useast-1.amazonaws.com |
| cloud9       | https://{random_id}.vfs.cloud9.{region}.amazonaws.com |
| mediastore   | https://{random_id}.data.mediastore.{region}.amazonaws.com |
| kinesisvideo | https://{random_id}.kinesisvideo.{region}.amazonaws.com |
| mediaconvert | https://{random_id}.mediaconvert.{region}.amazonaws.com |
| mediapackage | https://{random_id}.mediapackage.{region}.amazonaws.com/in/v1/{random_id}/channel |
### MultiCloud Governance
* [Cloud Custodian](https://github.com/cloud-custodian/cloud-custodian)
* [CloudQuary](https://github.com/cloudquery/cloudquery)
* [Cloudsploit](https://github.com/aquasecurity/cloudsploit)
* [ManageIQ by RedHat](https://github.com/ManageIQ/manageiq)
* [Mist.io](https://github.com/mistio/mist-ce)
* [NeuVector](https://github.com/neuvector/neuvector)
* [Triton by Joyent](https://github.com/joyent/triton)
## Kubernetes Operators
* Aqua
  * [Aqua Security Operator](https://operatorhub.io/operator/aqua)
  * [Starboard Operator](https://operatorhub.io/operator/starboard-operator)
* Misc
  * [Anchore - Anchore Engine Operator](https://operatorhub.io/operator/anchore-engine)
  * [Falco Security - Falco Operator](https://operatorhub.io/operator/falco)
  * [Quay - Project Quay Container Security](https://operatorhub.io/operator/project-quay-container-security-operator)
  * [Snyk - Snyk Operator](https://operatorhub.io/operator/snyk-operator)
  * [Splunk - Splunk Operator for Kubernetes](https://operatorhub.io/operator/splunk)
  * [Sysdig - Sysdig Agent Operator](https://operatorhub.io/operator/sysdig)

## Container Tools
* Anchore
  * [Anchore Engine](https://github.com/anchore/anchore-engine)
  * [Grype](https://github.com/anchore/grype)
  * [Kai](https://github.com/anchore/kai)
  * [Syft](https://github.com/anchore/syft)
* Aqua
  * [Cloudsploit](https://github.com/aquasecurity/cloudsploit)
  * [Kube-Bench](https://github.com/aquasecurity/kube-bench)
  * [Kube-Hunter](https://github.com/aquasecurity/kube-hunter)
  * [Kubectl-who-can](https://github.com/aquasecurity/kubectl-who-can)
  * [Trivy](https://github.com/aquasecurity/trivy)
* Misc
  * [Docker - Docker Bench for Security](https://github.com/docker/docker-bench-security)
  * [Elias - Dagda](https://github.com/eliasgranderubio/dagda/)
  * [Falco Security - Falco](https://github.com/falcosecurity/falco)
  * [Harbor - Harbor](https://github.com/goharbor/harbor)
  * [Quay - Clair](https://github.com/quay/clair)
  * [Snyk - Snyk](https://github.com/snyk/snyk)
  * [vchinnipilli - Kubestriker](https://github.com/vchinnipilli/kubestriker)
## Cloud Security Standards
* [ISO/IEC 27017:2015](https://www.iso.org/standard/43757.html)
* [ISO/IEC 27018:2019](https://www.iso.org/standard/76559.html)
* [MTCS SS 584](https://www.imda.gov.sg/industry-development/infrastructure/ict-standards-and-frameworks/mtcs-certification-scheme/multi-tier-cloud-security-certified-cloud-services)
* [CCM](https://cloudsecurityalliance.org/group/cloud-controls-matrix)
* [NIST 800-53](https://nvd.nist.gov/800-53)
## Learning
### Blogs
* [AWS Security](https://aws.amazon.com/blogs/security/)
* [Azure Security](https://www.microsoft.com/security/blog/azure-security/)
* [Dark Reading](https://www.darkreading.com/cloud-security.asp)
### Courses
* Oracle
  * [Oracle Cloud Security Administrator](https://learn.oracle.com/ols/learning-path/become-a-cloud-security-administrator/35644/38707)
* A Cloud Guru
  * Learning Paths
    * [AWS Security Path](https://learn.acloud.guru/learning-path/aws-security)
    * [Azure Security Path](https://learn.acloud.guru/learning-path/azure-security)
    * [GCP Security Path](https://learn.acloud.guru/learning-path/gcp-security)
### Labs
* [AWS Workshops](https://workshops.aws/categories/Security)
  * [AWS Identity: Using Amazon Cognito for serverless consumer apps](https://serverless-idm.awssecworkshops.com/)
  * [AWS Network Firewall Workshop](https://networkfirewall.workshop.aws/)
  * [AWS Networking Workshop](https://networking.workshop.aws/)
  * [Access Delegation](https://identity-round-robin.awssecworkshops.com/delegation/)
  * [Amazon VPC Endpoint Workshop](https://www.vpcendpointworkshop.com/)
  * [Build a Vulnerability Management Program Using AWS for AWS](https://vul-mgmt-program.awssecworkshops.com/)
  * [Data Discovery and Classification with Amazon Macie](https://data-discovery-and-classification.workshop.aws/)
  * [Data Protection](https://data-protection.awssecworkshops.com/)
  * [DevSecOps - Integrating security into your pipeline](https://devops.awssecworkshops.com/)
  * [Disaster Recovery on AWS](https://disaster-recovery.workshop.aws/)
  * [Finding and addressing Network Misconfigurations on AWS](https://validating-network-reachability.awssecworkshops.com/)
  * [Firewall Manager Service - WAF Policy](https://introduction-firewall-manager.workshop.aws/)
  * [Getting Hands on with Amazon GuardDuty](https://hands-on-guardduty.awssecworkshops.com/)
  * [Hands on Network Firewall Workshop](https://hands-on-network-firewall.workshop.aws/)
  * [Implementing DDoS Resiliency](https://ddos-protection-best-practices.workshop.aws/)
  * [Infrastructure Identity on AWS](https://idm-infrastructure.awssecworkshops.com/)
  * [Integrating security into your container pipeline](https://container-devsecops.awssecworkshops.com/)
  * [Integration, Prioritization, and Response with AWS Security Hub](https://pages.awscloud.com/Integration-Prioritization-and-Response-with-AWS-Security-Hub_2022_VW_s38e03-SID_OD)
  * [Introduction to WAF](https://introduction-to-waf.workshop.aws/)
  * [Permission boundaries: how to delegate permissions on AWS](https://identity-round-robin.awssecworkshops.com/permission-boundaries-advanced/)
  * [Protecting workloads on AWS from the instance to the edge](https://protecting-workloads.awssecworkshops.com/workshop/)
  * [Scaling threat detection and response on AWS](https://scaling-threat-detection.awssecworkshops.com/)
  * [Serverless Identity](https://identity-round-robin.awssecworkshops.com/serverless/)
* [PagerDuty Training Lab](https://sudo.pagerduty.com)
  * [PagerDuty Training GitHub](https://github.com/PagerDuty/security-training)
  * [PagerDuty Training for Engineers](https://sudo.pagerduty.com/for_engineers/)
  * [PagerDuty Training for Everyone: Part 1](https://sudo.pagerduty.com/for_everyone/)
  * [PagerDuty Training for Everyone: Part 2](https://sudo.pagerduty.com/for_everyone_part_ii/)
### Podcasts
* [Azure DevOps Podcast](http://azuredevopspodcast.clear-measure.com)
* [Cloud Security Podcast by Google](https://cloud.withgoogle.com/cloudsecurity/podcast/)
* [Security Now](https://twit.tv/shows/security-now)
### Vulnerable By Design
* [CloudGoat by Rhino Security Labs](https://github.com/RhinoSecurityLabs/cloudgoat)
* [ServerlessGoat by OWASP](https://github.com/OWASP/Serverless-Goat)
* [WrongSecrets by OWASP](https://github.com/commjoen/wrongsecrets)
## Certifications
* Cloud Vendors
  * [AWS Certified Security Specialty](https://aws.amazon.com/certification/certified-security-specialty/)
  * [Azure Security Engineer Associate](https://docs.microsoft.com/en-us/learn/certifications/azure-security-engineer/)
  * [Google Professional Cloud Security Engineer](https://cloud.google.com/certification/cloud-security-engineer)
  * [Oracle Cloud Platform Identity and Security Management](https://education.oracle.com/oracle-cloud-platform-identity-and-security-management-2020-certified-specialist/trackp_OCPISM2020CA)
* ISC<sup>2</sup> - International Information System Security Certification Consortium
  * [CCSP - Certified Cloud Security Professional](https://www.isc2.org/Certifications/CCSP)
* CSA - Cloud Security Alliance
  * [CCSK - Certificate of Cloud Security Knowledge](https://cloudsecurityalliance.org/education/ccsk/)
  * [CCAK - Certificate of Cloud Auditing Knowledge](https://cloudsecurityalliance.org/education/ccak/)
## Projects
### Alerting
* [411 by Etsy](https://github.com/etsy/411)
* [ElastAlert by Yelp](https://github.com/Yelp/elastalert)
* [StreamAlert by Airbnb](https://github.com/airbnb/streamalert)
### Automated Security Assessment
* [Prowler](https://github.com/prowler-cloud/prowler)
* [CloudFox](https://github.com/BishopFox/CloudFox)
* [SkyArk](https://github.com/cyberark/SkyArk)
* [Pacu](https://github.com/RhinoSecurityLabs/pacu)
* [Bucket Finder](https://digi.ninja/projects/bucket_finder.php)
* [Boto3](https://boto3.amazonaws.com/v1/documentation/api/latest/index.html)
* [Principal Mapper](https://github.com/nccgroup/PMapper)
* [ScoutSuite](https://github.com/nccgroup/ScoutSuite/wiki)
* [s3_objects_check](https://github.com/nccgroup/s3_objects_check)
* [cloudsplaining](https://github.com/salesforce/cloudsplaining)
* [weirdAAL](https://github.com/carnal0wnage/weirdAAL/wiki)
* [cloudmapper](https://github.com/duo-labs/cloudmapper)
* [NetSPI/AWS_Consoler](https://github.com/NetSPI/aws_consoler)
### Benchmarking
* [AWS Security Benchmark](https://github.com/awslabs/aws-security-benchmark)
### Data Loss Prevention
* [Git Secrets by AWS Labs](https://github.com/awslabs/git-secrets)
### Firewall Management
* globaldatanet
  * [AWS Firewall Factory](https://github.com/globaldatanet/aws-firewall-factory)
### Identity and Access Management
* AWS Labs
  * [AWS IAM Generator](https://github.com/awslabs/aws-iam-generator)
* Duo Labs
  * [Parliament](https://github.com/duo-labs/parliament)
  * [CloudTracker](https://github.com/duo-labs/cloudtracker)
* Netflix
  * [Aardvark](https://github.com/Netflix-Skunkworks/aardvark)
  * [ConsoleMe](https://github.com/Netflix/consoleme)
  * [PolicyUniverse](https://github.com/Netflix-Skunkworks/policyuniverse)
  * [Repokid](https://github.com/Netflix/Repokid)
* Pinterest
  * [Knox](https://github.com/pinterest/knox)
* Salesforce
  * [Policy Sentry](https://github.com/salesforce/policy_sentry/)
  * [CloudSplaining](https://github.com/salesforce/cloudsplaining)
  * [AWS-AllowLister](https://github.com/salesforce/aws-allowlister)
  * [Terraform for Policy Guru](https://github.com/salesforce/terraform-provider-policyguru)
* welldone.cloud
  * [aws-lint-iam-policies](https://github.com/welldone-cloud/aws-lint-iam-policies)
* Misc
  * [AWS Missing Tools by CloudAvail](https://github.com/cloudavail/aws-missing-tools)
  * [Awesome IAM List](https://github.com/kdeldycke/awesome-iam)
  * [Enumerate IAM by Andres Riancho](https://github.com/andresriancho/enumerate-iam)
  * [Kubernetes AWS IAM Authenticator by Kubernetes SIG](https://github.com/kubernetes-sigs/aws-iam-authenticator)
### Incident Response
* AWS
  * [AWS Incident Response Playbooks by AWS Samples](https://github.com/aws-samples/aws-incident-response-playbooks)
  * [AWS Security Hub Automated Response and Remediation](https://github.com/awslabs/aws-security-hub-automated-response-and-remediation)
* Netflix
  * [Dispatch by Netflix](https://github.com/Netflix/dispatch)
* PagerDuty
  * [PagerDuty Automated Remediation Docs](https://github.com/PagerDuty/automated-remediation-docs)
  * [PagerDuty Business Response Docs](https://github.com/PagerDuty/business-response-docs)
  * [PagerDuty DevSecOps Docs](https://github.com/PagerDuty/devsecops-docs)
  * [PagerDuty Full Case Ownership Docs](https://github.com/PagerDuty/full-case-ownership-docs)
  * [PagerDuty Full Service Ownership Docs](https://github.com/PagerDuty/full-service-ownership-docs)
  * [PagerDuty Going OnCall Docs](https://github.com/PagerDuty/goingoncall-docs)
  * [PagerDuty Incident Response Docs](https://github.com/PagerDuty/incident-response-docs)
  * [PagerDuty Operational Review Docs](https://github.com/PagerDuty/operational-review-docs)
  * [PagerDuty PostMortem Docs](https://github.com/PagerDuty/postmortem-docs)
  * [PagerDuty Retrospectives Docs](https://github.com/PagerDuty/retrospectives-docs)
  * [PagerDuty Stakeholder Communication Docs](https://github.com/PagerDuty/stakeholder-comms-docs)
* Velocidex
  * [Velociraptor](https://github.com/Velocidex/velociraptor) 
### Spring
* [Spring Cloud Security](https://github.com/dschadow/CloudSecurity)
### Threat modeling
* [ThreatModel for Amazon S3](https://github.com/trustoncloud/threatmodel-for-aws-s3) - Library of all the attack scenarios on Amazon S3 and how to mitigate them, following a risk-based approach
## Examples
### Ex. Automated Security Assessment
* [AWS Config Rules Repository](https://github.com/awslabs/aws-config-rules)
* [AWS Inspector Agent Autodeploy](https://github.com/awslabs/amazon-inspector-agent-autodeploy)
* [AWS Inspector Auto Remediation](https://github.com/awslabs/amazon-inspector-auto-remediate)
* [AWS Inspector Lambda Finding Processor](https://github.com/awslabs/amazon-inspector-finding-forwarder)
### Ex. Identity and Access Management
* [Amazon Cognito Streams connector for Amazon Redshift](https://github.com/awslabs/amazon-cognito-streams-sample)
### Ex. Logging
* [AWS Centralized Logging](https://github.com/awslabs/aws-centralized-logging)
* [AWS Config Snapshots to ElasticSearch](https://github.com/awslabs/aws-config-to-elasticsearch)
* [AWS CloudWatch Events Monitor Security Groups](https://github.com/awslabs/cwe-monitor-secgrp)
### Ex. Web Application Firewall
* [AWS WAF Sample](https://github.com/awslabs/aws-waf-sample)
* [AWS WAF Security Automations](https://github.com/awslabs/aws-waf-security-automations)
## Misc
* Other Awesome Lists
  * [Awesome Cloud Cost Control](https://github.com/Funkmyster/awesome-cloud-cost-control)
  * [Awesome Cloud Native Security](https://github.com/brant-ruan/awesome-cloud-native-security)
  * [Awesome Cloud Security](https://github.com/Funkmyster/awesome-cloud-security)
  * [Awesome IAM List](https://github.com/kdeldycke/awesome-iam)
  * [Awesome Incident Response List](https://github.com/meirwah/awesome-incident-response)
  * [Awesome Shodan Queries](https://github.com/jakejarvis/awesome-shodan-queries)
## Contribute
Contributions welcome! Read the [contribution guidelines](contributing.md) first.
## License
[![CC0](http://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](http://creativecommons.org/publicdomain/zero/1.0)

To the extent possible under law, Jacob Silva has waived all copyright and
related or neighboring rights to this work.
