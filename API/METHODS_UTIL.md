# Utility Methods
Utility methods created to help with various common scenarios

### util.BurnRagdoll(rag, burn_time, scorch)
Burns a player ragdoll, shows scorch marks, and automatically destroys the ragdoll unless it's been extinguished by water.\
*Realm:* Server\
*Added in:* 1.9.1\
*Parameters:*
- *rag* - The `prop_ragdoll` to set on fire
- *burn_time* - How long the ragdoll should burn for before being destroyed
- *scorch* - Whether scorch marks should be created under the ragdoll (Defaults to `true`)

### util.CanRoleSpawn(role)
Returns whether a role can be spawned either naturally at the start of a round or artificially.\
*Realm:* Client and Server\
*Added in:* 1.9.5\
*Parameters:*
- *role* - The role ID in question

### util.CanRoleSpawnArtificially(role)
Returns whether a role can be spawned artificially. (i.e. Spawned in a way other than naturally spawning when the role is enabled.)\
*Realm:* Client and Server\
*Added in:* 1.9.5\
*Parameters:*
- *role* - The role ID in question

### util.CanRoleSpawnNaturally(role)
Returns whether a role can be spawned naturally. (i.e. Spawned in at the start of the round if they are enabled or used in a role pack.)\
*Realm:* Client and Server\
*Added in:* 2.0.7\
*Parameters:*
- *role* - The role ID in question

### util.ExecFile(filePath, errorIfMissing)
Executes a file at the given path, relative to the root game location.\
*Realm:* Server\
*Added in:* 1.6.7\
*Parameters:*
- *filePath* - The path to the file to be executed, relative to the root game location
- *errorIfMissing* - Whether to throw an error if the file is missing (Defaults to `false`)

### util.FormattedList(tbl, formatting)
Turns a table of items into a string with commas and grammar.
*Realm:* Client and Server\
*Added in: 2.1.17\
*Parameters:*
- *tbl* - The table of items in question
- *formatting* - A function to apply formatting to each item in the provided table. (Optional, if not provided will just attempt to use table items as given)

### util.GetRoleIconPath(role_str, typ, ext, file_name_override)
Gets the path to a role's icon of the given type.\
*Realm:* Client and Server\
*Added in:* 2.0.7\
*Parameters:*
- *role_str* - The role string used in the icon path and name
- *typ* - The type of icon whose path is being found
- *ext* - The file extension to use in the role icon path
- *file_name_override* - The file name to use, appended to `{typ}_` when the path is built (Optional, defaults to the `{role_str}` value)
