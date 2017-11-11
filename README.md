PersistData
===========

Persistent store data at runtime in Unity3D. Hashmap behind the scenes, accept any kind of types. Singleton, keep data alive between scenes.

> It's under development, the syntax might change in the future. Even I try to make it safe please use it at your own risk.

## Usage example

Set data:
```csharp
PersistData.Instance.Set("test", "data");
```

Get data:
```csharp
string data = (string)PersistData.Instance.Get("test");
```

Test data:
```csharp
if (PersistData.Instance.Has("test")) {
    // Exists
}
```

Delete data:
```csharp
PersistData.Instance.Del("test");
```