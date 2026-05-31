# Aws-N8n-WorkFlow
# Awd n8n Lead Capture Workflow

## Overview
Automated lead capture system built with n8n, 
deployed on AWS EC2.

## Features
- Webhook receives form data
- Validates input with If node
- Stores leads in Google Sheets
- Sends automated Gmail response
- Error handling for invalid data

## Tech Stack
- n8n (workflow automation)
- AWS EC2 (Ubuntu 26.04, t3.micro)
- Google Sheets API
- Gmail API
- Docker

## AWS Deployment
- Instance: t3.micro (Sydney region)
- Public IP: 54.206.187.113
- Port: 5678
- Deployed via Docker

## Workflow Flow
Webhook → If → Google Sheets → Gmail → Response

## How to Test
Body: {
  "name": "Test",
  "email": "test@gmail.com", 
  "phone": "9876543210",
  "message": "Test message"
}


