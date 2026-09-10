# Mulchbutler rclone

Mulchbutler rclone is a personal, self-hosted file synchronization service. It
runs [rclone](https://rclone.org), an open-source command-line program for
copying and syncing files between local storage and cloud storage providers, on
a private server operated by the site owner.

## What this app does

The app connects a Google Drive account to an rclone installation running on the
owner's own server. Once connected, rclone can:

- Copy and sync files and folders between the server's local disk and Google Drive
- List the contents of Drive folders so that sync jobs can determine what has
  changed since the last run
- Upload new or modified files to Drive, and download files from Drive to the
  server
- Maintain scheduled backups of server data to Drive

All of this runs on a schedule set by the server owner. There is no web
interface, no hosted product, and no sign-up. The app exists so that rclone can
be authorized against Google Drive using its own OAuth client credentials
instead of rclone's shared default credentials.

## Why the app requests Google Drive access

rclone treats Google Drive as a storage backend, so it needs permission to read
and write files in the Drive account being synced. Without file-level access to
Drive, rclone cannot list folders to detect changes, upload backups, or restore
files. No other Google services are accessed, and no data is requested beyond
what a sync operation requires.

## Who can use it

This deployment is intended for the site owner's personal use. It is not offered
as a service to the public and there is no registration.

## Privacy

Read the [privacy policy](/privacy/) for details on what data the app accesses,
how it is used, and how it is stored.

## Contact

Questions about this app can be sent to the support address listed on the
OAuth consent screen.
