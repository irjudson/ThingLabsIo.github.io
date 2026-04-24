# ThingLabs.io

> **Historical Project** — The ThingLabs IoT workshop website (2015–2017). Preserved as a reference for the curriculum and workshop materials that accompanied the ThingLabs-IoT-Dashboard project.

The source for [thinglabs.io](http://thinglabs.io), a Jekyll-based educational website hosting hands-on IoT workshop curriculum. ThingLabs provided guided labs for developers learning to connect physical devices to cloud services, with a focus on Microsoft Azure IoT.

## What ThingLabs Was

ThingLabs was a community-driven initiative offering free, self-paced IoT workshop content. The site hosted step-by-step labs covering:

- **Node.js Connected Weather Station** -- Arduino Uno + sensors publishing telemetry to Azure IoT Hub
- **Windows 10 IoT Core / Raspberry Pi** -- C# apps on a connected nightlight using Azure services
- **Particle Photon** -- Wi-Fi connected device labs
- **ESP8266** -- low-cost Wi-Fi microcontroller workshops
- **Intel Edison** -- full-day deep-dive labs
- **ThingLabs for Windows** -- Windows 10 IoT Core specific curriculum

Labs covered the full stack: hardware wiring, firmware/Node.js code, Azure IoT Hub ingestion, stream analytics, Power BI visualization, and machine learning insights.

## Site Structure

```
pages/workshop/    # Workshop lab content organized by platform
pages/             # Supporting pages (setup guides, device info, schedule)
_config.yml        # Jekyll configuration (title, analytics, theme settings)
_data/             # Navigation and site data
_includes/         # Reusable HTML partials
_layouts/          # Page layout templates
assets/            # CSS, JS, fonts
images/            # Device photos and lab diagrams
```

## Building Locally

The site uses Jekyll with the `github-pages` gem.

```bash
# Install dependencies
bundle install

# Serve locally (development config)
bundle exec jekyll serve --config _config.yml,_config_dev.yml

# Or build for production
bundle exec jekyll build
```

The site will be available at `http://localhost:4000`.

## Related Projects

- [ThingLabs-IoT-Dashboard](https://github.com/ThingLabsIo/ThingLabs-IoT-Dashboard) -- the Node.js dashboard application used in the labs (25 forks)

**License:** MIT