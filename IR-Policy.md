# Incident response

See [CIO 2100.1L – GSA IT Security Policy](https://www.gsa.gov/cdnstatic/CIO_2100_1L_CHGE_1_CC040905_signed_PDF_version_7-15-2019.pdf) Chapter 4, _Policy on Operational Controls_, which covers:

* Awareness and Training (AT)
* Configuration Management (CM)
* Contingency Planning (CP)
* Incident Response (IR)
* Maintenance (MA)
* Media Protection (MP)
* Physical and Environmental Protection (PE)
* Personnel Security (PS)
* System and Information Integrity (SI)

The latest version can be found on the [GSA IT Security Policies](https://www.gsa.gov/about-us/organization/office-of-the-chief-information-officer/chief-information-security-officer-ciso/it-security-policies) page.

## Purpose

Iteratively reduce both the number of incidents as a proportion of our total information system inventory, and reduce the mean time to recover from incidents.

## Scope

See the **_Applicability_** section of the GSA IT Security Policy.

## Policy overlay

For information on roles and responsibilities, management commitment, coordination among organizational entities, compliance, reviews, and updates please see the [Technology Transformation Service's (TTS) Common Control Policy](https://github.com/18F/compliance-docs/blob/master/TTS-Common-Control-Policy.md).

## Procedures

The cloud.gov Program Manager organizes incident response training sessions, offered to the whole cloud.gov team at least annually, and requires that all Cloud Operations team members take the training. The training may be led by the Program Manager, a Cloud Operations team member, or another security specialist at 18F.

The cloud.gov team onboarding checklist (https://github.com/18F/cg-product/blob/master/OnboardingChecklist.md) requires that all team members take incident response training within 60 days of joining the team.

This training is a meeting reviewing and explaining the cloud.gov IR Guide (https://docs.cloud.gov/ops/security-ir/) and discussing questions and examples. The team takes notes on the training, stored in a Google Doc in the cloud.gov team Google Drive folder. The team records attendance in that document.

If the cloud.gov system changes in a radical way, the Program Manager adapts the incident response training to meet the needs of the new system. The Program Manager then requires Cloud Operations team members to take the training again.
The Program Manager requires all Cloud Operations team members to take the incident response training at least once a year.

See IR-2.

The cloud.gov team, as directed by the Program Manager, creates test plans and exercises in accordance to NIST 800-61, and presents these to the cloud.gov Authorizing Official for their approval.

cloud.gov tests its incident response capabilities with an annual table top exercise. The test takes the form of a teleconference (GSA Google Hangout) meeting where a security specialist (such as the Program Manager, a Cloud Operations team member, or another security specialist from 18F) guides the Cloud Operations team through a role-playing exercise with a simulated potential security incident. The team takes notes throughout the test, and afterward the team discusses the test and identifies weaknesses to fix with additional training or process improvements. The team files and tracks improvements with GitHub issues.

See IR-3, IR-3 (2).

cloud.gov implements automated processes to detect and analyze malicious activity within the platform. If these processes detect malicious activity, they automatically report the activity to the Cloud Operations team.

cloud.gov has an Incident Response Guide (https://docs.cloud.gov/ops/security-ir/) that documents the procedures that staff should take in the case of an incident, as required by the 18F and GSA Incident Response Policy.

See IR-4, IR-5, IR-6.

The Cloud Operations team implements automated processes such as ClamAV and Tripwire to detect anomalies. When these processes detect an anomaly, they escalate an alert to Cloud Operations team members using PagerDuty.

cloud.gov automatically stores logs so that Cloud Operations and GSA Information Security can access relevant information when investigating a potential incident. AWS level logs are automatically stored in CloudWatch Logs.

See IR-4 (1), IR-6 (1).

As described in the cloud.gov security incident response guide and contingency plan, Cloud Operations can notify customers about incidents and potential incidents using StatusPage (https://cloudgov.statuspage.io/), when this is appropriate for the incident. StatusPage allows customers to subscribe to updates by email or text message.

Customers can report potential incidents (and request support) via Slack or email, as documented at https://docs.cloud.gov/help/. The Security Incident Response guide explains to customers that they should email the cloud.gov support address if they encounter potential security problems (https://docs.cloud.gov/ops/security-ir/).

cloud.gov customers can subscribe to StatusPage to automatically receive alerts about the availability of cloud.gov services.

See IR-7, IR-7 (1).

As part of 18F, the cloud.gov team has direct and cooperative relationships with the Infrastructure team and the GSA Information Security team.
Within GSA Information Security, the cloud.gov team also works directly with its assigned ISSO, whose responsibility during incident response events facilitates cooperative relationships between cloud.gov’s incident response capability and external providers of information system protection capability.

GSA Information Security has direct relationships with other providers of federal incident response capability, inclusive of US-CERT.

See IR-7 (2).

The cloud.gov team has developed an Incident Response Guide (https://docs.cloud.gov/ops/security-ir/) to implement incident response capabilities.

The Incident Response Guide is continually reviewed and updated by the cloud.gov team. In addition, the cloud.gov team updates the IR Guide after it tests the guide, which happens at least annually and after any major system/organizational changes.

The cloud.gov team distributes changes to the Incident Response Guide to the whole cloud.gov team.

See IR-8.

The cloud.gov Incident Response directs cloud.gov team members to watch out for and immediately report any potential security incident, which includes reporting suspected information spills (such as sensitive or classified information in the wrong places). In the event of a suspected information spill, cloud.gov team members follow the reporting process in the cloud.gov Incident Response Guide.

The 18F Open Source Policy practices guide (which cloud.gov follows as part of 18F) at https://github.com/18F/open-source-policy/blob/master/practice.md#protecting-sensitive-information includes a reminder that spilled classified information must be reported via the response process.

The System Owner, Program Manager, and Cloud Operations team members have primary responsibility for implementing the actual response to security incidents, including technical measures. GSA Information Security is responsible for assisting the cloud.gov team in responding to security incidents.

See IR-9, IR-9 (1), IR-9 (2), IR-9 (3).

The cloud.gov Incident Response Guide identifies notification to parties exposed to unauthorized information of their obligations for handling that information among the long-term remediation steps to be recorded by the Incident Commander.

See IR-9 (4).