# StealthNetwork+ Discord Bot

A feature-rich Discord bot built for the StealthNetwork+ community, providing moderation tools, ticket management, and collaboration features.

## Features

### Moderation Commands
- `/ban` - Ban a user from the server
- `/kick` - Kick a user from the server
- `/timeout` - Temporarily timeout a user
- `/add-role` - Add a role to a user
- `/remove-role` - Remove a role from a user

### Development Commands
- `/push-update` - Send a development update to the dev chat
- `/dev-ping` - Ping developers for attention
- `/collab-request` - Create a collaboration request

### Community Commands
- `/announce` - Make a server announcement
- `/poll` - Create a poll with up to 5 options

### Ticket System
- Advanced ticket management with categories
- Staff claim system
- Ticket logging and archiving

## Setup

1. Clone the repository:
```bash
git clone https://github.com/yourusername/stealthnetworkbot.git
cd stealthnetworkbot
```

2. Install dependencies:
```bash
npm install
```

3. Create a `.env` file based on `.env.example`:
```env
DISCORD_TOKEN=your_discord_bot_token_here
GUILD_ID=your_discord_server_id_here
OWNER_ID=your_discord_user_id_here
NODE_ENV=development
DATABASE_PATH=./src/storage/stealthnetwork.sqlite
```

4. Configure server IDs:
Update `src/config/serverIds.ts` with your server's channel, role, and category IDs.

5. Build and run:
```bash
# Development
npm run dev

# Production
npm run build
npm start
```

## Development

### Project Structure
```
src/
├── Commands/           # Slash commands and handlers
├── config/            # Configuration files
├── database/          # Database models and connection
├── systems/           # Core systems (tickets, utils, etc.)
└── index.ts          # Main entry point
```

### Adding New Commands
1. Create command file in `src/Commands/`
2. Create handler in `src/Commands/handlers/`
3. Register in `src/Commands/index.ts`

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details. 