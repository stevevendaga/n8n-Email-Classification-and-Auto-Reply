# Email Classification and Auto Reply Workflow

## Overview
This n8n workflow automates email processing by classifying incoming emails as sponsorship inquiries and providing automated responses when appropriate. The workflow uses AI to analyze emails and respond professionally to potential sponsorship opportunities.

## Features
- **Automated Email Monitoring**: Continuously checks Gmail inbox using triggers
- **Sponsorship Detection**: Uses AI agent to identify sponsorship-related emails
- **Smart Response System**: Generates personalized responses for valid sponsorships
- **Professional Filtering**: Only responds to qualified inquiries based on content analysis

## Architecture

### 1. Trigger
- **Gmail Trigger**: Polls Gmail every minute for new messages

### 2. Data Processing
- **Edit Fields**: Formats email data into structured context
- **AI Agent**: Analyzes email content to determine sponsorship relevance
- **Structured Output Parser**: Validates AI response as JSON

### 3. Decision Logic
- **If Condition**: Routes emails based on sponsorship classification

### 4. Response Generation
- **OpenAI Node**: Creates professional HTML email responses
- **Gmail Node**: Sends replies to qualified sponsorship inquiries

### 5. Fallback
- **No Operation Node**: Handles non-sponsorship emails (no action)

## Configuration Requirements

### Credentials Needed
- **Gmail OAuth2**: For email integration
- **OpenAI API**: For AI-powered analysis and response generation

### Sponsorship Terms
The workflow includes predefined terms:
- Standalone Video: €800-€1,300
- Integrated Mention: €600
- Channel stats: 15,000+ subscribers, 3,000-10,000 average views

## How It Works
1. New email arrives → Gmail trigger activates
2. Email content is formatted and passed to AI agent
3. AI determines if email is sponsorship-related
4. If yes: Generate and send professional response
5. If no: Do nothing (email remains unprocessed)

## Customization
- Adjust polling frequency in Gmail Trigger settings
- Modify prompt instructions in AI Agent node
- Update sponsorship pricing in OpenAI message template
- Change AI model selection as needed