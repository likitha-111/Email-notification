# Email Notification System

An automated workflow system that monitors Gmail for incoming emails, sends real-time Slack notifications, and maintains comprehensive logs in Google Sheets.

## 📋 Project Overview

This project implements an end-to-end automated notification pipeline designed to:
- Monitor Gmail inbox for incoming emails
- Trigger automated workflows based on email events
- Send instant Slack notifications to team channels
- Store and track all notifications in Google Sheets for audit and reporting

## ✨ Features

### 1. Gmail Integration
- Automatically monitors specified Gmail inbox
- Triggers workflows on new incoming emails
- Filters emails based on custom criteria (sender, subject, keywords)
- Supports multiple Gmail accounts

### 2. Slack Notifications
- Sends real-time alerts to Slack channels
- Customizable message formatting
- Includes email details (sender, subject, timestamp)
- Error notifications for failed workflows

### 3. Google Sheets Logging
- Automatically records all notifications in Google Sheets
- Logs include:
  - Email details (sender, subject, date/time)
  - Notification status
  - Workflow execution status
  - Timestamps and error messages
- Easy-to-review audit trail for compliance and tracking

## 🚀 Getting Started

### Prerequisites
- Gmail account with API access enabled
- Slack workspace with bot permissions
- Google account with Sheets API access
- Required API keys and credentials

## 🔧 Configuration

Update the configuration file with your settings:
- Gmail inbox to monitor
- Slack channel for notifications
- Google Sheets spreadsheet ID
- Email filter criteria
- Notification schedule

## 📊 Workflow

```
Gmail Monitor → Email Detected → Workflow Triggered → Slack Notification → Google Sheets Logged
```


## 🔒 Security Considerations

- Store API keys in environment variables, not in code
- Use OAuth 2.0 for API authentication
- Implement rate limiting to prevent abuse
- Regularly rotate API credentials
- Monitor logs for suspicious activity
