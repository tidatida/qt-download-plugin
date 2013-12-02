# Qt Download Plugin

Resumable Qt download plugin.

See `DownloadInterface` for plugin methods and signals

## How to use

#### 1. Load plugin using `QPluginLoader`
#### 2. Set plugin parameters:

```
downloader.setQueueSize(size)
downloader.setFilePath(path)
downloader.setUserAgent(agent)
downloader.setExistPolicy(policy)
downloader.setPartialPolicy(policy)
```

alternatively one can use

```
downloader.setDefaultParameters();
```

#### 3. Start download using `append`

```
downloader.append(url);
```

## Example

`PluginHost` project shows examples how to use download plugin. Clone the project in the same directory as the plugin.
