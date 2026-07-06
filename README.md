# F1tasy 🏎️
A Formula 1 fantasy league manager.

## APIs
I chose Svelte for this project because of its simplicity in setting everything up, especially in terms of auth (Better Auth) and database features (drizzle). I plan on using OpenF1 for the statistics, but I'm still yet to learn more about this.

- [Svelte](https://svelte.dev/) - for the website, routing
- [Better Auth](https://better-auth.com/) - for signing up, logging in, tracking player
- [drizzle](https://orm.drizzle.team/) - for database, user information, driver information
- [OpenF1](https://openf1.org/) - for the F1 statistics (help players with choosing player)
- [Zod](https://zod.dev/) - TypeScript-first schema validation with static type inference

## App structure
In regards to Svelte, the pages will probably look something like this.

| Page Route   | Purpose           | Key functionality                                              |
| ------------ | ----------------- | -------------------------------------------------------------- |
| `/`          | Landing/Dashboard | User-specific view of their roster/standing                    |
| `/login`     | Auth              | Better Auth sign-in/sign-up forms                              |
| `/league`    | League Lobby      | List of all users and their team rankings                      |
| `/team`      | Team Manager      | Drag-and-drop or button-based interface to add/release drivers |
| `/market`    | Trade/Sign        | List available drivers/constructors with their *cost*          |
| `/resources` | Info              | Historical stats, rules, and F1 technical context              |
