# Rust Desktop App Template
A Desktop Application Base Project for building GUI Apps with Rust.
Using tauri with native webviews, and combining tauri features from the various examples.
For a better starting point for building Graphical Desktop Applications in Rust.
It uses MetroUI and Metro Icon Font libraries for basic widgets and styling.


Main target OS is Windows. Secondary target is Linux. 
Default GUI style: black theme.


For an overview of all the icons that can be used: https://metroui.org.ua/icons.html



Work In Progress...




## Development with live server
Reload the html content without needing to close and reopen the application.

Use live server from https://crates.io/crates/live-server


### Install
$ cargo install live-server


### Usage
In VSCode, right click on the index.html file, and open a new terminal. Run command: $ live-server -H 127.0.0.1 -p 5500 -o

If you want to change the port, change the 5500 in the live-server command and also in the tauri.conf.json:

```
"build": {
    "devPath": "http://127.0.0.1:5500/index.html",
    "distDir": "../src"
}
```

Note that the production path distDir, is still set to the html source directory src, and does not use the live server.
If you do not want to use a live-server, you can set the devPath to the same as the distDir.

Security warning: 

Do not use the live server for production. As it would open the application up to a lot of security issues. You would have to make it https with SSL certificates and the lot. Keep the distDir on `"../src"` and it will be just fine.


### Help
$ live-server --help



