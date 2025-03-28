# Automated Paper Distribution

This repository includes an automated system for distributing your scientific paper without relying on traditional publishing channels. The system works by generating machine-readable metadata, RSS feeds, and registry entries that can be discovered and indexed by automated systems.

## How It Works

When you publish a new version of your paper (by creating a GitHub Release or manually triggering the workflow), the following happens automatically:

1. **Metadata Generation**: Structured data about your paper is created in multiple formats
2. **RSS Feed Updates**: Your paper is added to an RSS feed that others can subscribe to
3. **Registry Submission**: Your paper is submitted to a decentralized registry of GitHub-based papers
4. **Social Media Announcements**: If configured, announcements are posted to scientific social media

## Setting Up Distribution

### Basic Setup

The distribution system is pre-configured and will work automatically when you:

1. Fill out your paper's metadata in `paper/metadata.yml`
2. Create a GitHub Release when your paper is ready

### Social Media Integration (Optional)

To enable social media announcements:

1. Go to your repository settings → Secrets and variables → Actions
2. Add the following secrets:
   - `MASTODON_TOKEN`: Your Mastodon API token
   - `MASTODON_INSTANCE`: Your Mastodon instance (e.g., `fosstodon.org`)

### Manual Triggering

You can manually trigger the distribution workflow:

1. Go to the "Actions" tab in your repository
2. Select the "Distribute Paper" workflow
3. Click "Run workflow"
4. Enter the version (e.g., "v1.0.0") and indicate if it's a major update

## Discovery

Your paper will be discoverable through:

1. **RSS Feed**: Available at `https://yourusername.github.io/your-repo/dist/feed.xml`
2. **Metadata**: Machine-readable metadata at `https://yourusername.github.io/your-repo/dist/metadata.json`
3. **Local Registry**: A registry entry at `https://yourusername.github.io/your-repo/dist/registry/index.json`

As more papers use this system, discovery tools and aggregators will be developed to make finding papers easier.

## Customization

You can customize the distribution process by:

1. Editing the scripts in `.github/scripts/`
2. Modifying the workflow in `.github/workflows/distribute-paper.yml`
3. Adding additional distribution channels

## Future Development

This distribution system will evolve over time. Future enhancements may include:

- Integration with specialized scientific search engines
- Support for more social media platforms
- Creation of a centralized registry for all GitHub-based papers
- Citation notification system
