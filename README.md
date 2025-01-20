Here's a `README.md` file for your GitHub repository that explains how to use the `setup-ssh.sh` script:


# Server Setup

This repository contains a collection of server setup scripts, including configuration for SSH keys and other server-related utilities. The primary script is `setup-ssh.sh`, which automates the process of adding SSH public keys to a server.

## `setup-ssh.sh`

The `setup-ssh.sh` script is designed to add an SSH public key to the `~/.ssh/authorized_keys` file on your server. It ensures that the server is properly configured to allow passwordless SSH login using the provided key.

### Features:
- Adds an SSH public key to the server's `~/.ssh/authorized_keys` file.
- Creates the `.ssh` directory if it doesn't exist.
- Ensures the proper permissions for the `.ssh` directory and the `authorized_keys` file.

## Usage

### Option 1: Download and Execute the Script via `curl`

You can directly download and run the script on your server using the following `curl` command:

```bash
curl -sSL https://raw.githubusercontent.com/asadrahman03/server-setup/refs/heads/main/setup-ssh.sh | bash
```

### Option 2: Download and Execute the Script via `wget`

Alternatively, you can use `wget` to download and run the script:

```bash
wget -qO- https://raw.githubusercontent.com/asadrahman03/server-setup/refs/heads/main/setup-ssh.sh | bash
```

### Manual Usage

1. Clone the repository to your server:

   ```bash
   git clone https://github.com/asadrahman03/server-setup.git
   cd server-setup
   ```

2. Make the script executable:

   ```bash
   chmod +x setup-ssh.sh
   ```

3. Run the script:

   ```bash
   ./setup-ssh.sh
   ```

This will add your SSH public key to the server's `authorized_keys` file and set the correct permissions for the `.ssh` folder.

## Requirements

- A Linux-based server with SSH access.
- Your SSH public key that you want to add to the server.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
```

### Explanation:
1. **Overview of the repository**: Describes the repository's purpose and the functionality of the main script.
2. **Usage**: Explains how to use the script, both through direct execution via `curl` or `wget`, and manually.
3. **Requirements**: Lists prerequisites for running the script.
4. **License**: Suggests using the MIT License, but feel free to adjust it if necessary.
