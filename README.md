# chitty-pkg-google-calendar

Chitty Workspace marketplace package — Full Google Calendar integration with 5 tools.

## Requirements

- [Chitty Workspace](https://github.com/MTPython406/Chitty-Workspace) (required)
- [Chitty SDK](https://github.com/MTPython406/chitty-sdk) (`pip install chitty-sdk`)

## Tools

| Tool | Description |
|------|-------------|
| `gcal_list` | List & search — upcoming events, past lookup, search by person/topic/date |
| `gcal_create` | Create events with validation, attendee controls, multi-calendar |
| `gcal_freebusy` | Find available time slots across multiple calendars |
| `gcal_update` | Partial event updates via PATCH (reschedule, rename, modify) |
| `gcal_delete` | Cancel events with optional notification (feature-gated) |

## Search Examples

- `query="Mike Miller" days_back=90` — Find past meetings with Mike
- `query="budget review"` — Find events by topic
- `days_back=30` — Show all events from last month

## Security

- 4 feature flags: create, update, delete (off), invite attendees (off)
- Input validation, attendee email checks, calendar ID validation
- Notification control: explicit opt-in
- Configurable allowed calendar IDs

## Installation

Install via the Chitty Workspace Marketplace tab, or manually:

```bash
# Clone into your Chitty marketplace directory
git clone https://github.com/MTPython406/chitty-pkg-google-calendar.git \
  ~/.chitty-workspace/data/tools/marketplace/google-calendar
```

## License

MIT — see [Chitty Workspace](https://github.com/MTPython406/Chitty-Workspace) for full license.

Built by [DataVisions.ai](https://datavisions.ai) | [chitty.ai](https://chitty.ai)
