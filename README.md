# sentry.mobi

A work-in-progress alternative frontend to Sentry.

Right now it can view organizations, projects and a projects issues.

1. `make`
2. `target/debug/sentry-mobi`
3. get a user API token from sentry (User Settings)
4. Log in at `http://localhost:3000`

## Design goals

* Should work on small screens and low-end devices. **Must** run smoothly on
  Android devices from 10 years ago (Android 9, Samsung Galaxy S8)

  * Therefore, JavaScript is used to progressively enhance at most (probably
    going to use HTMX)

* Main user scenario is responding to and viewing alerts on mobile. Tracing
  views etc are unlikely to be implemented because they're too complex.

  * Therefore, link to full UI where it's convenient.

* Some kind of story for compliance, as unlike other alternative frontends
  we're dealing with sensitive data. Self-hostable on local device.

  * Therefore, self-contained binary.

## LICENSE

MIT
