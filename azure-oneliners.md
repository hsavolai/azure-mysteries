# List of azure oneliners and such

## OL-1: Testing service principal credentials

```bash
az login --service-principal --username "[CLIENT ID]" --password "[CLIENT SECRET]" --tenant "[TENANT ID]"
# Next, see if required entitites are accessible with ie. az group list 
```

## OL-2: Substring searching for users based on the Display name
```bash
az ad user list --query "[?contains(displayName,'Harri')]"
# Note! Case insensitive matching does not exist. Hint! userPrincipalName might have a lower case version of the name. 
```
