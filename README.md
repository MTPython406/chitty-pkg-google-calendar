# chitty-pkg-google-calendar

Chitty Marketplace package — Full Google Calendar integration (5 tools).

## Tools
- **List & Search** — Upcoming events, past lookup, search by person/topic/date range
- **Create** — Create events with validation, attendee controls, multi-calendar
- **FreeBusy** — Find available time slots across multiple calendars
- **Update** — Partial event updates via PATCH (reschedule, rename, modify)
- **Delete** — Cancel events with optional notification (feature-gated)

## Search Examples
- `query="Mike Miller" days_back=90` — Find past meetings with Mike
- `query="budget review"` — Find events by topic
- `days_back=30` — Show all events from last month

## Security
- 4 feature flags: create, update, delete (off), invite attendees (off)
- Input validation, attendee email checks, calendar ID validation
- Notification control: explicit opt-in
- Configurable allowed calendar IDs

## Dependencies
- `chitty-sdk`

## License
MIT
