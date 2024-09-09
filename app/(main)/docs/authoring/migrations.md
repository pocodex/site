## Migrations

pocodex supports PocketBase-compatible migrations, allowing you to manage your plugin's database changes easily. To enable migration support, simply move the `migrate(...)` command from the PocketBase-generated migration file into your plugin's migration array. pocodex will handle the migration process during installation and uninstallation.

### Migration Guidelines

- **Modify only your own collections and tables**: Never modify outside tables or collections.
- **Ensure backward compatibility**: Avoid removing old columns or changing column types to incompatible types.
- **Order of application**: pocodex applies migrations during installation in array order, after the normal PocketBase migrations have run.
- **Uninstallation**: All down migrations are applied when a plugin is uninstalled.
- **Plugin table modifications**: Encourage users not to modify your plugin's tables, as this can cause PocketBase to generate migrations for tables that may not exist for other users.

With these features, pocodex provides a robust system for managing PocketBase plugins in a way that's safe and efficient.
