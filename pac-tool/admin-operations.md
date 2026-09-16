# Reset the environment

https://learn.microsoft.com/en-us/power-platform/developer/cli/reference/admin

`pac admin list` - List all environments in the Power Platform tenant.

`pac admin reset --environment "YOUR_ENVIRONMENT_ID_HERE"` - Reset the specified environment to its default state. This operation will delete all data, customizations, and configurations in the environment. Use this command with caution, as it cannot be undone.

## Optional Customization Arguments

You can append additional flags to configure the environment as it resets:
--name: Change the display name of the environment.
--currency: Define the base currency for the Dataverse instance (e.g., USD).
--templates: Specify a Dynamics 365 template to install if needed.
--purpose: Provide a description of the environment's purpose.

`pac admin reset --environment "1234abcd-56ef-78gh-90ij-1234567890kl" --name "Fresh Dev Environment" --currency "USD"` - Reset the specified environment and set a new name and currency for it. This command will also delete all data, customizations, and configurations in the environment. Use this command with caution, as it cannot be undone.

`pac admin status` - Check the status of the reset operation. This command will provide information on whether the reset is in progress, completed, or if there were any errors during the process.