# How to update Go version

### 1. Uninstall the exisiting version

To uninstall, delete the /usr/local/go directory by:

```$ sudo rm -rf /usr/local/go```

### 2. Install the new version
Go to the downloads page and download the binary release suitable for your system.

```https://go.dev/dl/```

Example: ```wget https://go.dev/dl/go1.18.1.linux-amd64.tar.gz```

### 3. Extract the archive file
To extract the archive file:

$ sudo tar -C /usr/local -xzf go1.8.1.linux-amd64.tar.gz

### 4. Make sure that your PATH contains /usr/local/go/bin
```$ echo $PATH | grep "/usr/local/go/bin"```
