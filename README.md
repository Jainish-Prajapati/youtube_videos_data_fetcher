# YouTube Videos Data Fetcher

It is a Rust-based CLI tool to fetch YouTube video data using a channel ID and save it to a CSV file. It uses the YouTube Data API v3 and is designed for quick and efficient extraction of video information such as video ID, title, description, and published date.

## Features
- Fetch video data using a YouTube channel ID.
- Save data to a CSV file for further use (e.g., GenAI applications or data analysis).

## Dependencies
The project uses the following Rust crates:
- `reqwest` (v0.11): For making HTTP requests (with JSON support).
- `tokio` (v1): For asynchronous runtime (with full features enabled).
- `serde_json` (v1.0): For handling JSON data.
- `csv` (v1.1): For writing data to CSV files.
- `dotenv` (v0.15): For loading environment variables (e.g., API keys).

## Requirements
- **YouTube Data API v3 Key**: Obtain an API key from the [Google Cloud Console](https://console.cloud.google.com/).
- **Channel ID**: The unique identifier of the YouTube channel you want to fetch video data from.

## Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/Jainish-Prajapati/youtube_videos_data_fetcher.git
   cd youtube_videos_data_fetcher
   ```

2. Save YouTube Data API v3 in ```.env``` file & initialize ```channel_id``` variable with channel id of which you want data(can get using: [TunePocket](https://www.tunepocket.com/youtube-channel-id-finder/))

3. Run Project(install rust before this step):
    ```bash
    cargo run
    ```

4. You will get videos_data.csv file after that

## Contributions
Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/Jainish-Prajapati/youtube_videos_data_fetcher/issues) or submit a pull request.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

## Acknowledgments
- [YouTube Data API](https://developers.google.com/youtube/v3) for providing the data.
- [TunePocket](https://www.tunepocket.com/youtube-channel-id-finder/) for the convenient channel ID finder tool.
- The Rust community for their excellent documentation and support.

Happy coding! 🚀