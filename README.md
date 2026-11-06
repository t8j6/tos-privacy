# Jail Bot

Server moderation bot with a jail system. One slash command (`/setup`), everything else runs
through your own chat prefix (e.g. `.jail @user reason`).

## 1. Create the bot (Discord Developer Portal)

1. https://discord.com/developers/applications \u2192 **New Application**
2. **Bot** tab \u2192 **Reset Token** \u2192 copy it, this is your `DISCORD_TOKEN`
3. Still on the **Bot** tab, scroll to **Privileged Gateway Intents** and turn ON:
   - **Server Members Intent**
   - **Message Content Intent**
   (both are required \u2014 without them the bot can't read `.jail` messages or fetch member roles)
4. **General Information** tab \u2192 copy the **Application ID**, this is your `CLIENT_ID`
5. **OAuth2 \u2192 URL Generator**:
   - Scopes: `bot` and `applications.commands`
   - Bot Permissions: `Manage Roles`, `Manage Channels`, `View Channels`, `Send Messages`,
     `Manage Messages`, `Read Message History`, `Embed Links`
   - Open the generated link to invite the bot to your server

**Important:** after inviting, go to Server Settings \u2192 Roles and drag the bot's own role **above**
the jail role and above any role it needs to strip from members. Discord bots can only manage
roles positioned below their own highest role.

## 2. Run it locally (optional, to test)

```bash
npm install
cp .env.example .env
# paste your token + client id into .env
npm run deploy   # registers /setup (global \u2014 can take up to ~1h to appear everywhere)
npm start
```

Then run `/setup` in your server as an Administrator.

## 3. Hosting it for free, 24/7

Quick correction from earlier in this chat: **Railway is not permanently free anymore** \u2014
it's a one-time $5 trial credit, then $5/month. Not what you asked for, so skip it here.

For "always on, free, no credit card, don't have to think about it," these fit better:

- **Wispbyte** (wispbyte.com) \u2014 free tier, no credit card, no manual renewal
- **Bot-Hosting.net** \u2014 one free bot, no credit card, no renewal step

Both are smaller, Discord-bot-specific hosts rather than big cloud platforms \u2014 fine for a bot
this size, just not as battle-tested as something like Railway. If the bot ever needs more
power, that's when a small paid VPS starts making sense.

**One thing that matters regardless of host:** this bot saves its data as JSON files in the
`data/` folder. Whichever host you pick, make sure that folder isn't wiped when the bot restarts
or redeploys \u2014 otherwise `/unjail` won't remember who had which roles. If you tell me which
host you land on, I can walk you through that specific step.

## Commands

- `/setup` \u2014 admin-only, configures prefix, jail role, jail channel, moderator roles, log channel
- `<prefix>jail @user reason` or `<prefix>jail <user id> reason`
- `<prefix>unjail @user [reason]`
