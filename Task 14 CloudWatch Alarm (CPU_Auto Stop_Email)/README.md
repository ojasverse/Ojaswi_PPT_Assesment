# Task 14: CloudWatch Alarm for CPU Utilization

## Objective
To automatically stop EC2 instance and send email when CPU exceeds 70%.

## Services Used
- CloudWatch
- EC2
- SNS

## Implementation Steps
1. Created SNS topic and email subscription.
2. Created CloudWatch alarm with 70% CPU threshold.
3. Configured alarm action to stop EC2.
4. Tested by generating CPU load.

## Proof
- Screenshot 1: CloudWatch Alarm Configuration
- Screenshot 2: Email Notification

## Outcome
EC2 automatically stopped when CPU exceeded 70%.
