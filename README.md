# Carepal Liver Cirrhosis Chatbot

## Overview

This Flutter-based chatbot is a component of the Carepal app, specifically designed to assist patients with liver cirrhosis. The chatbot utilizes Google's Gemini AI, which is being fine-tuned to understand and respond to queries related to liver cirrhosis data and patient questions.

## Features

- Personalized responses to patient queries about liver cirrhosis
- Ability to summarize clinical notes from MIMIC database
- User-friendly interface for easy interaction
- Support for both text and image inputs
- Chat history storage for continuity of care using flutter Hive database

## Prerequisites

Before running this app, you need to:

1. Have Flutter installed on your development machine
2. Obtain a Gemini API key from Google AI Studio

## Setup

1. Clone this repository:

```bash

```

2. Navigate to the project directory:

```bash
cd carepal-liver-cirrhosis-chatbot
```
3. Install dependencies:

```bash
flutter pub get
```
4. Set up your Gemini API key:

- Open `lib/api/api_service.dart`
- Replace `YOUR_ACTUAL_API_KEY_HERE` with your Gemini API key:
  ```dart
  class ApiService {
    static const apiKey = 'YOUR_ACTUAL_API_KEY_HERE';
  }
  ```

5. Run the app:
```bash
flutter run
```

## Usage

- Launch the app and start a new chat session
- Type your questions about liver cirrhosis or upload relevant images
- Receive AI-generated responses based on the latest medical knowledge and your personal data
- The current gemini 1.5 pro model is also really good in summarizing clinical notes. you can try by posting a sample clinical note from mimic datasets.

## AI Model Information

The chatbot uses a Gemini AI model fine-tuned in Google AI Studio to better understand liver cirrhosis data and patient questions. It has demonstrated proficiency in summarizing clinical notes from the MIMIC (Medical Information Mart for Intensive Care) database.

## Note for Developers

This chatbot is currently in development and will be integrated into the larger Carepal app ecosystem. Future updates will include more specialized features for liver cirrhosis management and broader health monitoring capabilities.

## Getting a Gemini API Key

To run this app, you need to obtain a Gemini API key from Google AI Studio:

1. Visit [Google AI Studio](https://makersuite.google.com/app/apikey)
2. Sign in with your Google account
3. Create a new API key
4. Use this key in the `ApiService` class as mentioned in the Setup section

## Screenshots
![alt text](<Screenshot 2024-09-30 at 9.36.43 PM.png>) ![alt text](<Screenshot 2024-09-30 at 9.36.52 PM.png>) ![alt text](<Screenshot 2024-09-30 at 9.37.02 PM.png>) ![alt text](<Screenshot 2024-09-30 at 9.37.41 PM.png>)


