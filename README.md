# Amazon Product Price Tracking System

A cloud-based application to track and analyze Amazon product prices, monitor historical trends, and notify users of price drops.

## Features

- **Track Prices**: Monitor prices for popular products or user-submitted Amazon URLs.
- **Analyze Trends**: View historical price data for up to 120 days.
- **Notifications**: Receive alerts via email or push notifications for price drops.
- **User-Friendly Interface**: Intuitive web interface for managing tracked products and alerts.
- **Scalable Architecture**: Built on Google Cloud Platform (GCP) for high scalability and reliability.

## Tech Stack

### Backend
- **Google Cloud Functions**: For web scraping and backend logic.
- **Bright Data / Keepa API**: For scraping Amazon product prices and metadata.

### Data Management
- **Google Firestore**: To store product metadata and user preferences.
- **Google BigQuery**: For storing and analyzing price data.
- **Google Cloud Storage**: For storing product images and metadata.

### Frontend
- **React** (or Vue.js): For building the user interface, hosted on **Firebase Hosting**.

### Notifications
- **Firebase Cloud Messaging**: For push notifications.
- **SendGrid**: For email notifications.

## System Workflow

1. **Data Collection**:
   - Scrape product data using Bright Data or Keepa APIs.
   - Store metadata and pricing information in Firestore and BigQuery.

2. **Data Analysis**:
   - Analyze trends like average price, minimum price, and price fluctuations.

3. **User Interaction**:
   - Users interact with a web interface to search, view trends, and set up notifications.

4. **Notifications**:
   - Notify users when prices drop below their specified thresholds.

## Setup Instructions

### Prerequisites
- Google Cloud Platform (GCP) account.
- API keys for Bright Data or Keepa.
- Node.js and Firebase CLI for frontend setup.
