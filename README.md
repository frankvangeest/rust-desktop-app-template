# Rust Desktop App Template
A Desktop Application Base Project for building GUI Apps with Rust.
Using tauri with native webviews, and combining tauri features from the various examples.
For a better starting point for building Graphical Desktop Applications in Rust.
It uses MetroUI and Metro Icon Font libraries for basic widgets and styling.

Main target OS is Windows. Secondary target is Linux. 
Default GUI style: black theme.

For an overview of all the icons that can be used: https://metroui.org.ua/icons.html

Work In Progress...




Development with live server.
Reload the html content without needing to close and reopen the application.

Use live server from https://crates.io/crates/live-server
Install
$ cargo install live-server
Usage
In VSCode, right click on the index.html file, and open a new terminal. Run command: $ live-server -H 127.0.0.1 -p 5500 -o
Help
$ live-server --help



