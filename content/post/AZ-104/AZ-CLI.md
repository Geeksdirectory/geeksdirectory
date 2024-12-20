

# Start the vm

```
az vm start --resource-group personal --name MyServer
```

# Stop

```
az vm stop --resource-group personal --name MyServer
```

# Create an vm 

```
az vm create \
  --resource-group MyResourceGroup \
  --name MySpotVM \
  --image UbuntuLTS \
  --priority Spot \
  --eviction-policy Deallocate \
  --size Standard_B1s \
  --admin-username azureuser \
  --ssh-key-value ~/.ssh/id_rsa.pub
```

