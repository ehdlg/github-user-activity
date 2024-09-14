# GitHub User Activity CLI

This is a simple Python-based CLI application that fetches and displays the recent activity
of a specified GitHub user. This project is part of
[roadmap.sh's GitHub User Activity Project](https://roadmap.sh/projects/github-user-activity),
and the goal of this program is to practice making HTTP requests and using Python modules like
`requests` , while also getting familiar with `match` cases for handling different types of events.

## Features

- Fetches recent activity of a GitHub user using the GitHub Events API.
- Displays events such as push commits, opened issues, starred repositories, and more.
- Validates that a GitHub username is provided and that the user exists.
- Option to specify a limit on the number of recent events to display.
- Error handling, including missing username, user not found and API error scenarios.

## Installation

1. **Clone the repository:**

   ```bash
   git clone git@github.com:ehdlg/github-user-activity.git
   ```

2. **Navigate to the project directory**:

   ```bash
   cd github-user-activity
   ```

3. **Install the dependencies:**
   Make sure you have pip installed and then run:
   ```bash
   pip install -r requirements.txt
   ```

## Usage

To run the application, use the following command:

```bash
python main.py <username> [filter]
```

Where:

- < username >: The GitHub username for which you want to fetch recent activity.
- [filter] (optional): A filter to specify the number of events to display. If not provided, the last 30 events will be shown.

### Examples

- Display recent activity of a user without a limit:

  ```bash
  python main.py example_user
  ```

- Display the first 10 recent events of a user:

  ```bash
  python main.py example_user 10
  ```
