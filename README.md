# Tove Tools Skill

## Overview

Adds behavior guidance for working with the Tove Tools connector's CSV transform tool: correctly locating a product CSV in Google Drive when it isn't uploaded directly, and presenting the transform tool's results without misrepresenting the data.

## Components

- **Skill: shopify-csv-prep** — teaches Claude how to source the input CSV (uploaded file or Google Drive) and how to present `transform_csv`'s output: link only, no unsolicited data-quality review.

## Setup

This plugin does **not** include the Tove Tools MCP server itself — it only adds the skill. Before the skill is useful, connect the Tove Tools connector separately:

1. In Claude, go to Settings → Connectors → Add
2. Add Tove Tools using the connection details and API key provided by Sunny.
3. Once connected, this plugin's skill applies automatically whenever a product CSV needs to be prepped for Shopify.

## Usage

Just describe what's needed in plain language — "get this CSV ready for Shopify," "clean up this product export," "make this uploadable to Shopify" — whether the file is uploaded directly or referenced from Google Drive. No need to name the tool or connector.
