# Task 12: Website Down Alert using CloudWatch Canary & SNS

## Objective
To monitor website uptime and send alert when site is down.

## Services Used
- CloudWatch Synthetics (Canary)
- SNS
- IAM

## Implementation Steps
1. Created SNS topic with email subscription.
2. Created CloudWatch Canary.
3. Configured failure threshold.
4. Linked SNS to alarm.
5. Tested by stopping website.

## Proof
- Screenshot 1: Canary Configuration
- Screenshot 2: CloudWatch Alarm
- Screenshot 3: Email Alert

## Outcome
Successfully implemented automated website downtime alert system.
