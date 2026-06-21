# GitHub Profile Analyzer API

## Overview

A Node.js and Express.js API that analyzes GitHub user profiles using the GitHub Public API and stores useful insights in a MySQL database.

## Features

* Fetch GitHub profile data by username
* Calculate useful profile insights
* Store analysis results in MySQL
* Get all analyzed profiles
* Get a single analyzed profile

## Tech Stack

* Node.js
* Express.js
* MySQL
* GitHub REST API
* Axios

## Installation

1. Clone the repository

```bash
git clone https://github.com/Ravichandrikalanka/github-profile-analyzer.git
```

2. Install dependencies

```bash
npm install
```

3. Create a `.env` file

```env
PORT=5000
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=R@vichandrika25
DB_NAME=github_analyzer
```

4. Run the application

```bash
node app.js
```

## API Endpoints

### Analyze GitHub Profile

GET /api/profile/:username

Example:

GET /api/profile/octocat

### Get All Profiles

GET /api/profiles

### Get Single Profile

GET /api/profiles/:username

Example:

GET /api/profiles/octocat

## Database Schema

Table: profiles

Columns:

* id
* github_id
* username
* name
* bio
* followers
* following
* public_repos
* total_stars
* profile_url
* avatar_url
* analyzed_at

## Author

Ravi Chandrika
