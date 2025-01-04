# WP Debug Wizard 🧙‍♂️

A magical command-line tool for debugging WordPress websites with AI assistance! ✨

## Features 🌟

- Full site backup (files + database)
- WordPress health checks
- Automated debug mode configuration
- Real-time log monitoring
- AI-powered error analysis (using Claude AI)
- Beautiful console output
- Interactive debugging workflow

## Prerequisites 🛠️

- macOS
- Homebrew
- SSH access to your WordPress server
- Anthropic API key (for Claude AI integration)

## Installation 🚀

1. Clone the repository:

```bash
git clone https://github.com/gbechtold/wp-debug-wizard.git
cd wp-debug-wizard
```

2. Install dependencies:

```bash
brew install curl jq zip mysql
```

3. Make the script executable:

```bash
chmod +x wp-debug.sh
```

4. Copy and configure the environment file:

```bash
cp .env.example .env
nano .env  # Edit with your settings
```

## Usage 🎯

Start debugging with a single command:

```bash
./wp-debug.sh
```

The wizard will guide you through the entire debugging process:

1. 🔄 Creates a full backup
2. 🏥 Checks site health
3. 🔍 Enables debug mode
4. 📝 Monitors debug log
5. 🤖 Analyzes errors with AI

## Configuration ⚙️

Edit `.env` file with your settings:

```env
ANTHROPIC_API_KEY=your_key_here
SITE_URL=https://your-wordpress-site.com
REMOTE_USER=your-ssh-user
REMOTE_HOST=your-ssh-host
REMOTE_PATH=/path/to/wordpress
DB_NAME=wordpress_db
DB_USER=db_user
DB_PASSWORD=db_password
BACKUP_PATH=./backups
```

## Contributing 🤝

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License 📜

MIT License - feel free to use in your projects!
