# Printer Server for UmbrelOS

A CUPS-based print server that lets you share USB printers over your home network.

## Install via Community App Store

1. Open your Umbrel dashboard
2. Go to **App Store**
3. Scroll to **Community App Stores**
4. Add this store URL: `https://github.com/YOUR_USERNAME/umbrel-community-store`
5. Find **Printer Server** and click Install

## Usage

1. Plug a USB printer into your Umbrel
2. Open the Printer Server app from your Umbrel dashboard
3. Click **Administration** → **Add Printer**
4. Select your printer and follow the prompts

## Default Login

| Field | Value |
|---|---|
| Username | `admin` |
| Password | `admin` |

Change the password immediately after first login! Set `ADMIN_PASSWORD` env variable in the app settings.

## Build & Publish

```bash
# Fork the community app store repo
# https://github.com/getumbrel/umbrel-community-app-store

# Add your app directory
cp -r printer-server/ /path/to/umbrel-community-app-store/

# Update umbrel-app-store.yml in the root
# Then submit a Pull Request
```

## Directory structure

```
umbrel-community-store/
├── umbrel-app-store.yml          # Store metadata
└── printer-server/
    ├── umbrel-app.yml            # App metadata (Umbrel App Store format)
    └── docker-compose.yml        # Docker services
```
