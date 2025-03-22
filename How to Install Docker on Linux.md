### Step 1: Install Required Dependencies

Run the following command to install the necessary dependencies for Docker installation:

```bash
sudo apt install apt-transport-https ca-certificates curl gnupg
```

- **apt-transport-https**: Allows the use of HTTPS to fetch packages.
- **ca-certificates**: Installs necessary certificates for secure communication.
- **curl**: Used to fetch files from URLs.
- **gnupg**: A tool to manage GPG keys for secure software installation.

### Step 2: Add Docker GPG Key and Repository

1. Fetch and add Docker's official GPG key:

```bash
curl -fsSL https://download.docker.com/linux/debian/gpg | sudo gpg --dearmor -o /usr/share/keyrings/docker.gpg
```

Downloads Docker’s GPG key and stores it locally for verification during installation.

2. Add Docker's official repository to your system's package manager:

```bash
echo "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker.gpg] https://download.docker.com/linux/ubuntu noble stable" | sudo tee /etc/apt/sources.list.d/docker.list /dev/null
```

Adds Docker's repository to your system to allow installation of Docker packages.

### Step 3: Install Docker Desktop

1. Download the latest Docker Desktop DEB package from [Docker's official site](https://desktop.docker.com/linux/main/amd64/docker-desktop-amd64.deb?utm_source=docker&utm_medium=webreferral&utm_campaign=docs-driven-download-linux-amd64).
2. Install the downloaded package using the following commands:

```bash
sudo apt-get update
sudo apt-get install ./docker-desktop-amd64.deb
```

- **sudo apt-get update**: Refreshes the package database to ensure the latest packages are available.
- **sudo apt-get install ./docker-desktop-amd64.deb**: Installs Docker Desktop from the downloaded DEB package.
