# Manage auth profiles
https://learn.microsoft.com/en-us/power-platform/developer/cli/introduction

## Create an authentication profile
`pac auth create` - Create a new authentication profile for your Power Platform environment.

`pac auth create --environment "<environment-name>"` - Create a new authentication profile for a specific environment.

`pac auth create --name "<profile-name>"` - Create a new authentication profile with a specific name.

## List and Select profiles
`pac auth list` - List all authentication profiles.

`pac auth select --index 2` - Select an authentication profile by its index in the list.


## Delete an authentication profile
`pac auth delete --index <index_number>` - Delete an authentication profile by its index in the list.

`pac auth delete --name <profile_name>` - Delete an authentication profile by its name.