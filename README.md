# OpenSea NFT Stealer
This simple script automatically downloads entire NFT collections from OpenSea. Now you can collect JPEGs without burning the planet down!

## Usage
1. Clone this [repository](https://github.com/DOFER998/OpenSea-NFT-Stealer.git).
2. Run the script: `python3 main.py [collections and flags]`

## Note
You can specify as many collections as you want to download. For example, if you want to download all the BAYC and CryptoPunks NFTs, do this: `python3 main.py boredapeyachtclub cryptopunks`.
By default, all downloaded collections will be saved in a directory called `collections`. Due to a restriction placed on the OpenSea API, a maximum of 10,000 NFTs will be downloaded from a single collection.

The script currently supports image, video, and audio NFTs. Other types of files will still be downloaded, but they will be saved with a `.bin` extension. Feel free to open an issue if you encounter this and we can add support for that file type.

### Configuration Flags
In addition to specifying collections to download, you can also configure the behavior of the script with flags.

* `--quiet`: Do not output the name and last price of individual NFTs.
* `--download-dir=<dir>`: Set the directory to save NFTs to. Replace \<dir\> with the path to the directory. The directory will be created if it doesn't exist.