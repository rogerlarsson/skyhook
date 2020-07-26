# Skyhook
Send and recieve files securely through the IPFS network

# Overview
Skyhook is a command-line tool that allows the user to securely share files over the IPFS network.
It features:
-   Seamless file encryption and decryption using AES-256
-   Local history of file names, hashes, keys and dates which can be both imported and exported easily
-   Ability to run off both local and remote IPFS nodes

# Usage
Simply running Skyhook with no arguments gives the user a list of available commands:

```
    skyhook clear history - Delete everything from history
    skyhook list history - List all entries in history
    skyhook list keys - List all files and their corresponding encryption keys
    
    skyhook search [file name] - Search history for entries matching [file name]
    skyhook delete [hash] - Delete entries specified by [hash] from history
    skyhook save [hash] - Save a single history entry specified by [hash] to the local directory
    
    skyhook import [path] - Import history from a location specified by [path]
    skyhook export [path] - Export history to a location specified by [path]
    
    skyhook upload [file name] - Upload a file specified by [file name] from the current working directory to the IPFS network
    skyhook download [hash] - Download a file specified by [hash] from the IPFS network

```

# Requirements
The only requirement for running Skyhook is the ipfs-api module for Python 3, which can be installed by running:

```
pip3 install ipfs-api
```

or

```
pip3 install --user ipfs-api
```

# Roadmap
-   Port Skyhook to Windows
-   Create a GUI version of Skyhook

# Final Note
Current iteration of Skyhook is also hosted on IPFS itself. It is available here: https://ipfs.io/ipfs/QmPumiCCYXPCJVuaQBgTknv8znhxzMcetL6WcTSBYKVMgg
