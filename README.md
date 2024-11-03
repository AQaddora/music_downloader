# Music Downloader 🎶

**Music Downloader** is a Python tool that downloads music from YouTube and automatically embeds metadata, album artwork, and lyrics from Genius. Perfect for building your offline music library with well-organized tags and rich media.

## Features

- **Downloads audio** from YouTube as MP3
- **Embeds metadata** like title, artist, album, and release date
- **Fetches album artwork** and attaches it to the MP3
- **Adds lyrics** automatically from Genius
- Works with most Python environments and media players

## Installation

You can install Music Downloader directly from PyPI:

```bash
pip install music_downloader
```

## Requirements

- Python 3.7 or higher
- YouTube audio extraction and metadata libraries (automatically installed with the package)

## Usage

Once installed, use `music-downloader` directly from the command line:

```bash
music-downloader "Song Title"
```

By default, files are saved in your Music directory, but you can specify a custom directory with the `--output_dir` option:

```bash
music-downloader "Song Title" --output_dir "/path/to/save/music"
```

### Example

```bash
music-downloader "Let Me Down Slowly Alec Benjamin"
```

This will:
1. Search YouTube for the official video of **"Let Me Down Slowly" by Alec Benjamin**.
2. Download the audio as an MP3.
3. Fetch metadata, album artwork, and lyrics from Genius.
4. Embed all metadata and save the file.

### Command-Line Options

- `song_name`: The title of the song you want to download.
- `--output_dir`: Custom directory to save the downloaded audio. Defaults to `~/Music`.

## Development

If you'd like to contribute or experiment with the code, clone the repository and install dependencies:

```bash
git clone https://github.com/yourusername/music_downloader.git
cd music_downloader
pip install -r requirements.txt
```

### Running Locally

To run the downloader locally:

```bash
python -m music_downloader.downloader "Song Title"
```

## License

This project is licensed under the MIT License.

## Acknowledgments

- Uses [yt-dlp](https://github.com/yt-dlp/yt-dlp) for downloading YouTube audio.
- Metadata and lyrics from [Genius](https://genius.com/).

## Support

For issues or feature requests, please open an issue on [GitHub](https://github.com/AQaddora/music_downloader/issues).
