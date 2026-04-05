"# Infrastructure Monitoring Dashboard

A minimal, clean dashboard for monitoring cloud infrastructure status.

## Features

- Environment status badge (healthy/degraded/critical)
- Summary cards showing instance counts by health status
- Instance table with CPU usage and health indicators
- Auto-refresh every 10 seconds
- No frameworks - pure HTML, CSS, and vanilla JavaScript

## Usage

Open `index.html` in a browser or serve it via any static file server.

## API Endpoint

The dashboard fetches data from the configured API endpoint. Expected format:

```json
{
  "environment_status": "healthy | degraded | critical",
  "timestamp": "ISO-8601 string",
  "summary": {
    "healthy": 5,
    "warning": 2,
    "critical": 1,
    "unknown": 0
  },
  "instances": [
    {
      "instance_id": "i-0001-abc123",
      "cpu": 45,
      "health": "healthy"
    }
  ]
}
```" 
