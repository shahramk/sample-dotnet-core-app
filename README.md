
# sample-dotnet-core-app

  

* run **dotnet new mvc sample-dotnet-app** to create a simple app.

* add manifest.yml:

```
    ---
    applications:
    - name: sample-dotnet-app
    memory: 256M
    buildpack: dotnet_core_buildpack
```

**Note:** it works with the current external dotnet core buildpack. but if I build a new buildpack:
```
    buildpack-packager build --any-stack
```

it fails to push the app.
