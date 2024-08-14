# Reachinbox Web Application

## Overview

This project is a web application developed for Reachinbox. It features a user-friendly interface to manage and interact with emails. Key functionalities include theme toggling, email management, and detailed views. The application integrates with Reachinbox APIs to fetch and manage email data.

## Features

- **Sidebar Navigation**: Provides quick access to various sections of the application.
- **TopBar**: Displays the current workspace and includes a theme toggle button.
- **Main Page**: Shows email threads, details of selected emails, and additional information.
- **Right Section**: Displays lead details and activity history.
- **SubView**: Placeholder view shown when there are no emails.
- **Custom Mail**: Allows users to compose and send replies.
- **Delete PopUp**: Confirms the deletion of emails.
- **Theme Toggle**: Switches between dark and light modes.

## Installation

1. **Clone the Repository**

   ```bash
   https://github.com/Abdul8971/ReachInBox-Frontend-assignment.git 

   ```

1. **Navigate to the Project Directory**

   bash

   Copy code

   `cd reachinbox`

1. **Install Dependencies**

   bash

   Copy code

   `npm install`

1. **Start the Development Server**

   bash

   Copy code

   `npm run dev`

   The application will be available at `http://localhost:5173`.

## API Endpoints

### 1\. **List Email Threads**

- **Endpoint**: `GET /api/v1/onebox/list`
- **Description**: Retrieves a list of email threads.
- **Headers**:
  - `Authorization`: Bearer token

### 2\. **Reply to Email Thread**

- **Endpoint**: `POST /api/v1/onebox/reply/{threadId}`
- **Description**: Sends a reply to a specified email thread.
- **Headers**:
  - `Authorization`: Bearer token
- **Request Body**:

  json

  Copy code

  `{
  "to": "recipient@example.com",
  "from": "sender@example.com",
  "subject": "Subject of the email",
  "body": "Body of the email"
}`

### 3\. **Reset Email Data**

- **Endpoint**: `GET /api/v1/onebox/reset`
- **Description**: Resets the email data (e.g., for testing purposes).
- **Headers**:
  - `Authorization`: Bearer token


## Figma Design

- [Reachinbox Design](https://www.figma.com/design/uECxqvFhEx9dn4ZuO7wqmu/Reachinbox-Assignment?node-id=1-20869&t=ZY1VyRCEYZB8EyvA-0)

## API Documentation

- [Postman API Documentation](https://documenter.getpostman.com/view/30630244/2sA2rCTMKr#f45cb7f3-d007-4df5-83f4-ea598d3e5015)
