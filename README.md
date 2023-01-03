# KHInsider CLI Album Downloader
This repository contains a simple script for the purpose of downloading all songs of an album in [KHInsider](https://downloads.khinsider.com/) without the need of an account or permission to download all at once.

It also gives normalized names to the songs in the form of "XX Name of song.format", with XX being an Integer with the same ammount of digits at the number of songs. Example:
```
- 4 Songs -> 1 digit number
- 43 Songs -> 2 digit number
- 140 Songs -> 3 digit number
```

## Usage
Clone the repository in your desired location, create a dotenv file and set the `ROOT_DOWNLOAD_DIR` variable to the desired root directory for your downloads

Make the file executable with

 **`chmod +x ./khicad`**

Execute the script using the `-u` flag for the full url of the album you want to download hosted on [KHInsider](https://downloads.khinsider.com/), the `-n` flag for the Album name, which will be the name of the folder created in `ROOT_DOWNLOAD_DIR`, and the `-f` flag for the song format.

And you are good to go, enjoy!

## Example

![image](https://user-images.githubusercontent.com/121802206/210351230-f5610177-1985-43b8-ad41-4b34dff7c707.png)

# Missing Features

```
- Propperly identify total album size for selected format
```
