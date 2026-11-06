# Privacy Policy for SSS Moderation

Last updated: 5 November 2026

SSS Moderation ("the Bot") is a Discord bot for moderation, tickets, giveaways, logging and server protection. This policy explains what data the Bot processes, why, how long it is kept and what rights you have. By using the Bot or being a member of a server that uses it, you acknowledge this policy.

## 1. Who is responsible

The Bot is operated by an individual developer ("we", "us").

Contact for all privacy questions and requests: **snow.public@proton.me**

## 2. Overview

- The Bot only works in Discord servers where a server owner or administrator has added it.
- We do not sell personal data, we do not use it for advertising and we do not build profiles for third parties.
- Most data the Bot stores is created by the server's own moderators and settings. The server owner decides which features and log channels are used.

## 3. Data the Bot processes today

### 3.1 Moderation records
- Discord user IDs of the moderator and of the affected user
- Type of action (ban, temporary ban, softban, kick, mute, unmute, warning, lock, unlock, purge and so on), reason, duration, date and status
- Case numbers and warnings (deleted warnings are only marked as deleted)
- Counters of how often a moderator used certain commands

### 3.2 Server settings
- Server ID, command prefix, role IDs and channel IDs
- Settings for welcome and goodbye messages, anti-nuke modules, log channels and trusted bot IDs

### 3.3 Member history
- When a member joined or left the server (only from the time the Bot was added)
- Known nickname changes and role changes (role IDs)

### 3.4 Logs
- Moderation actions are written to a log channel chosen by the server owner.
- If the server owner sets a **passive log channel**, the Bot logs events such as message edits and deletions, joins and leaves, nickname and role changes, timeouts, voice channel joins and leaves, and changes to channels, roles, bans, emojis, threads, webhooks, invites and server settings.
- To show what a message said when it is edited or deleted, the Bot keeps a temporary copy of messages: message ID, channel ID, author ID, message text and links to attachments. **Copies are deleted automatically after 7 days**, and a copy is removed once its deletion has been logged. Copies are only made while a passive log channel is set.

### 3.5 Tickets
- The ticket creator's ID, the reason entered, claim status and timestamps
- When a ticket is closed, the Bot reads the messages of the ticket channel (up to the latest 1,000) and sends them as a text file to the server's transcript channel. The Bot does not keep the transcript text itself.

### 3.6 Giveaways
- Discord user IDs of participants, so that winners can be drawn

### 3.7 Anti-nuke and recovery
- Counters of server-changing actions per user (for example bans or channel deletions) with timestamps. Counters are deleted after 2 days.
- Snapshots of channels and roles (names, positions, permission settings) so that deleted items can be restored. A snapshot of a deleted item is deleted after 7 days.

### 3.8 Data that is processed but not stored
- Message text is read to recognise commands that start with the server's prefix and to detect mass mentions (@everyone and @here).
- The Bot may send direct messages (for example to tell a user about a ban or warning). It does not read direct messages.

## 4. Data the Bot may process in the future

Discord bots commonly offer more features. We may add some of them later, for example: automatic moderation filters (scanning messages for words, links, invites or spam), levels and experience points, economy or virtual currency, reaction roles, custom commands, reminders, polls, birthdays, starboards, suggestions and reports, appeals, member verification, music or voice features, welcome images that use avatars and usernames, statistics and analytics, a web dashboard (with Discord login, which may involve OAuth tokens, cookies and IP addresses) and optional paid features (payments handled by an external payment provider; we would not store card details).

Before a feature that processes new kinds of personal data goes live, we will update this policy and the date at the top.

## 5. What the Bot does not collect

Passwords, payment card data, email addresses of members, location data and voice recordings. The Bot does not read direct messages.

## 6. Why the data is used

- To provide the features the server owner has set up (moderation, tickets, giveaways, logging, protection)
- To keep records of moderation actions for the server team
- To protect servers against abuse, spam and attacks such as mass deletion of channels
- To keep the Bot running, find errors and improve it

If the GDPR applies, the legal basis is our legitimate interest and that of the server owner in moderating and protecting the community (Art. 6(1)(f) GDPR). Where a feature requires consent, we will ask for it.

## 7. Who can see the data

- **Server staff:** Logs, cases, warnings and transcripts are shown in Discord channels chosen by the server owner. Anyone who can read those channels can see them.
- **Hosting provider:** The Bot runs at a third-party hosting provider (currently Wispbyte), which stores the Bot's database and files.
- **Discord:** Data is processed through Discord's platform under Discord's own terms and privacy policy.
- **Authorities:** We may disclose data if required by law or to protect rights and safety.

We do not sell data and we do not share it with data brokers.

## 8. International transfers

Discord and the hosting provider may process data outside your country, including outside the EEA or the UK. We rely on the safeguards of these providers.

## 9. How long data is kept

- Passive log message copies: 7 days
- Anti-nuke counters: 2 days
- Channel and role snapshots of deleted items: 7 days
- Moderation records, warnings, member history, ticket and giveaway records, and server settings: as long as the Bot is used in the server, or until you ask us to delete them
- Backups, if any, are deleted on a regular basis

## 10. Your rights

You can ask us at **snow.public@proton.me** to
- tell you which data we hold about you,
- correct it,
- delete it,
- restrict or stop processing it, or
- give you a copy of it.

Please include your Discord user ID. We may need to verify that the request comes from you. Depending on where you live (for example the EEA, the UK or California), you may have further rights, including the right to complain to a data protection authority. We do not sell personal information.

Moderation records may be kept where there is a legitimate reason, for example to prevent abuse or to document a ban. Server owners can remove the Bot at any time and can ask us to delete all data of their server.

## 11. Security

The Bot's token and database are kept on a protected server and access is limited to the operator. No system is perfectly secure, so we cannot guarantee absolute security. If we learn of a breach that affects you, we will act as the law requires.

## 12. Children

Discord requires users to be at least 13 years old (or older where local law requires). The Bot is not directed at younger children and we do not knowingly process their data. Contact us if you believe a child's data was stored, and we will delete it.

## 13. Changes

We may update this policy. The date at the top shows the latest version. Continued use of the Bot after a change means you accept the new version.

## 14. Contact

snow.public@proton.me
