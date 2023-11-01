## Rebaser: Auto-Rebase Your Git Branches

`rebaser` is a command-line utility that automatically rebases your feature branch whenever the `main` branch is updated. This script runs indefinitely, checking for updates to the `main` branch every 15 minutes.

### Prerequisites

- Python 3.x installed
- Git installed
- Terminal access to the repository you want to monitor

### Installation

1. Clone this repository or download the `rebaser` script.
2. Make the script executable:
    ```bash
    chmod +x rebaser
    ```
3. Copy the executable script to a directory in your PATH, for example:
    ```bash
    cp rebaser /usr/local/bin/
    ```

### Usage

Navigate to the terminal and run the `rebaser` script by specifying the path to the local repository and the name of the feature branch you want to auto-rebase:

```bash
rebaser /path/to/local/repo feature_branch_name
```

For example:

```bash
rebaser /Users/johndoe/projects/my_repo my_feature_branch
```

The script will run indefinitely and check for updates to the `main` branch of the specified repository every 15 minutes. If an update is detected, it will automatically rebase your feature branch and push the changes.

### Stopping the Script

To stop the script, you can simply press `Ctrl + C` in the terminal where it's running.

---

Feel free to adjust the language or add any additional details you think might be helpful!