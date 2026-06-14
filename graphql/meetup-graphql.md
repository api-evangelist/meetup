# Meetup GraphQL API

The Meetup GraphQL API is a single-endpoint API that provides access to Meetup's community platform data, including groups, events, members, RSVPs, venues, photos, and Pro network management. It is available to developers building applications on top of Meetup's ecosystem and is gated behind a Meetup Pro subscription for full access to features such as Pro network analytics, group management, and event publishing workflows.

The schema exposes a rich type system centered around four primary entities: Group, Event, Member, and ProNetwork. Queries allow searching for events and groups by keyword and location, fetching individual resources by ID or URL name, retrieving personalized recommendations, and accessing the authenticated member's own data. Mutations support the full lifecycle of event and group management, including creating, editing, announcing, and deleting events; managing RSVPs; uploading photos; and publishing group drafts.

Authentication is handled via OAuth 2.0, supporting Server Flow, Refresh Token Flow, JWT Flow, and Implicit Flow. Access tokens are passed as Bearer tokens in the Authorization HTTP header. The API is rate-limited to 500 query points per 60-second window. Introspection is available at the endpoint.

**Endpoint:** https://api.meetup.com/gql-ext

**Documentation:** https://www.meetup.com/graphql/

**References:**

- Documentation: https://www.meetup.com/graphql/
- GettingStarted: https://www.meetup.com/graphql/guide/
- Authentication: https://www.meetup.com/graphql/authentication/
- Playground: https://www.meetup.com/api/playground/
- Reference: https://www.meetup.com/graphql/
