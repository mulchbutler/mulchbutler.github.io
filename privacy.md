# Privacy Policy

Last updated: September 10, 2026

This policy describes how Mulchbutler rclone handles data. Mulchbutler rclone is
a personal, self-hosted deployment of [rclone](https://rclone.org) operated by
the owner of goldreilly.com. See the [home page](/) for a description of what
the app does.

## What data the app accesses

When a Google account is connected, the app receives an OAuth access token and
refresh token that allow it to access files in that account's Google Drive. It
uses this access to list, read, upload, and modify files and folders as part of
sync and backup operations requested by the server operator.

The app does not request or access Gmail, Contacts, Calendar, or any other
Google service.

## How the data is used

Google user data is used for one purpose only: performing the file
synchronization and backup operations described on the home page. File contents
pass through the server in order to be copied between local storage and Google
Drive.

The app does not use Google user data for advertising, profiling, training
machine learning models, or any purpose unrelated to file synchronization.

## How the data is stored

OAuth tokens are stored in the rclone configuration file on the server's local
disk, readable only by the operating system account that runs rclone. File
contents are stored on the server only where the operator has configured a sync
destination, and in temporary files during transfer.

There is no application database, and no analytics or tracking of any kind. The
app keeps no request logs beyond what the operating system and rclone record
locally for troubleshooting.

## How the data is shared

Google user data is never sold, transferred, or disclosed to third parties. The
only parties involved in a transfer are Google's APIs and the operator's own
server.

## Data retention and deletion

Access to a Google account can be revoked at any time from the
[Google Account permissions page](https://myaccount.google.com/permissions),
which immediately invalidates the app's tokens. Stored tokens are also deleted
when the rclone remote is removed from the server's configuration. Files already
copied to the server can be deleted by the operator on request.

## Limited Use disclosure

Mulchbutler rclone's use and transfer of information received from Google APIs
adheres to the
[Google API Services User Data Policy](https://developers.google.com/terms/api-services-user-data-policy),
including the Limited Use requirements.

## Changes to this policy

Any changes to this policy will be published on this page with an updated date
above.

## Contact

Questions about this policy can be sent to the support email address listed on
the app's OAuth consent screen.
