# azureml-irisexample

## Setting up your environment

- Install conda
- Install Azure CLI
- For dataset support in the SDK, install .NET core https://aka.ms/dotnet-install-linux, for WSL this is what I used:
    ```sudo apt-get update; \ sudo apt-get install -y apt-transport-https && \ sudo apt-get update && \ sudo apt-get install -y aspnetcore-runtime-2.1```
- Conda create environment

## Using the CLI

Register model
```
az ml model create --file registermodel.yml
```

Deploy model
```
az ml online-endpoint create --file deployment.yml
```

