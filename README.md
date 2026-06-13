# Meetup

Meetup is a community event platform that connects people with shared interests through in-person and online group meetings. Its GraphQL API provides programmatic access to group events, members, RSVPs, venue information, and community activity data for developers building integrations with the Meetup platform.

## API

Meetup provides a single-endpoint GraphQL API available to Meetup Pro subscribers. The API supports querying group and event data, managing RSVPs (called Tickets in the current API version), publishing events, uploading photos, and searching across Pro networks.

- **Endpoint:** `https://api.meetup.com/gql-ext`
- **API Type:** GraphQL
- **Authentication:** OAuth 2.0 (Bearer token)
- **Rate Limit:** 500 query points per 60-second window
- **Playground:** https://www.meetup.com/api/playground/

## Documentation

- [API Introduction](https://www.meetup.com/graphql/)
- [API Guide](https://www.meetup.com/graphql/guide/)
- [Authentication](https://www.meetup.com/graphql/authentication/)
- [Support](https://www.meetup.com/graphql/support/)
- [Help Center - API User Guide](https://help.meetup.com/hc/en-us/sections/41453323105549)

## Authentication

The Meetup API uses OAuth 2.0. Four flows are supported:

- **Server Flow** - for server-side applications
- **Refresh Token Flow** - for renewing expired tokens
- **JWT Flow** - for server-to-server interactions
- **Implicit Flow** - for browser-based JavaScript clients

OAuth endpoints:
- Authorization: `https://secure.meetup.com/oauth2/authorize`
- Token: `https://secure.meetup.com/oauth2/access`

## Plans

API access requires a **Meetup Pro** subscription (starting at $55/group/month). The Standard plan ($29.99/month) does not include API access.

## Repository Contents

- `apis.yml` - APIs.json 0.19 provider profile
- `plans/plans.yml` - Subscription plan details
- `rate-limits/rate-limits.yml` - Rate limiting details
- `finops/finops.yml` - Financial operations and cost information
