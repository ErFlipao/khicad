# KHInsider CLI Album Downloader
This repository contains a simple script for the purpose of downloading all songs of an album in [KHInsider](https://downloads.khinsider.com/) without the need of an account or permission to download all at once.

It also gives normalized names to the songs in the form of "XX Name of song.format", with XX being a 2 digit number. If there are more than 99 songs, the order in the download directory may not be ideal.

## Usage
Clone the repository in your desired location, create a dotenv file and set the `ROOT_DOWNLOAD_DIR` variable to the desired root directory for your downloads

Make the file executable with

 **`chmod +x ./khicad`**

Execute the script and enter the full url of the album you want to download hosted on [KHInsider](https://downloads.khinsider.com/), the Album name, which will be the folder in the `albumdir`, and select the song format `(mp3/flac)`

And you are good to go, enjoy!

## Example

![image](https://user-images.githubusercontent.com/121802206/210231663-85b6cd05-afc6-4c06-93b2-e32faacb35c4.png)

# Missing Features

File types offered automatic detection. It curently works with mp3 and flac, but it won't tell you if those formats are available. If there are two formats and the latter is WAV, the script will tell detect it as flac when choosing file format but will not download since the extension is not flac.
