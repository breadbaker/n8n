# n8n

This repository contains example resources for building workflows in [n8n](https://n8n.io/).

## Softwash lead qualifier workflow

The `workflows/softwash-lead-qualifier.json` file is a basic starting point for handling SMS leads. The flow uses Twilio nodes to receive incoming text messages, asks the sender for their details, and forwards the collected information to your number.

To use it:

1. Import the JSON file into your n8n instance.
2. Configure the Twilio credentials and replace `+YOUR_TWILIO_NUMBER` and `+MY_NUMBER` with the correct phone numbers.
3. Activate the workflow.

Incoming messages will prompt the lead for their name, phone number, and address. Once the data is captured, n8n sends you a summary text so you can follow up.
