# Godot GIF Parser
GDScript wrapper for loading GIF files from a `PackedByteArray` buffer and transforming them to an `AnimatedTexture`.

## Motivation
All Godot GIF Parser libraries I have come across work on files on the hard drive. My goal was to make a parser that also works with streamlined file buffers directly read from an online source.

## Installation and Usage
Add this repository as a submodule via `git submodule add http://DavidLokison/godot-gif-parser gif-parser`. Make sure to `git submodule update --init --recursive` afterwards.

Then, load and instanciate the script and call the `read(data: PackedByteArray) -> AnimatedTexture` method and pass it the loaded file or data stream content.

## Credits
The script is mainly based on the work of [godot-gif-importer](https://github.com/vbousquet/godot-gif-importer), which I updated to Godot 4.3 stable and reformatted to be used as a submodule. A plugin version is being worked on.

This script also uses [godot-gif-lzw](https://github.com/DavidLokison/godot-gif-lzw), forked from [here](https://github.com/jegor377/godot-gif-lzw), as a submodule.

## Contributing
Any contribution is greatly appreciated!
