# List of azure oneliners and such

## OL-1: Testing service principal credentials

```bash
az login --service-principal --username "[CLIENT ID]" --password "[CLIENT SECRET]" --tenant "[TENANT ID]"
# Next, see if required entitites are accessible with ie. az group list 
```
