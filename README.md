<p align="center">
  <a href="https://aoi.js.org">
    <img width="100" src="https://github.com/aoijs/website/blob/master/assets/images/aoimusic.png?raw=true" alt="aoi.music">
  </a>
</p>

<h1 align="center">@fluffy/aoi.music</h1>

A powerful TypeScript-based JavaScript library that adds music-related properties and lays a solid foundation for music operations in fluffy.js. 

## 🚀 Setup

To get started with @aoijs/aoi.music, follow these simple steps:

1. Install fluffy.music via npm:

   ```bash
   npm install fluffy.music
   ```

2. Import the Manager class and create a new instance:

   ```javascript
   const { Manager } = require("fluffy.music");
   
   const manager = new Manager({
      devOptions: {
         debug: false, // Set to true for debugging purposes
      },
      searchOptions: {
         soundcloudClientId: "<YOUR_SOUNDCLOUD_CLIENT_ID>",
         youtubeAuth: true, // Options: TRUE or FALSE, default: TRUE
         youtubegl: "<YOUR_YOUTUBE_COUNTRY_CODE>", // default: US
         youtubeClient: "WEB", // Options: "WEB" | "ANDROID" | "YTMUSIC_ANDROID" | "YTMUSIC" | "YTSTUDIO_ANDROID" | "TV_EMBEDDED", default: WEB
      },
      requestOptions: {
         offsetTimeout: 1500, // Timeout in milliseconds for searching and skipping, default: 500
         soundcloudLikeTrackLimit: 10, // Limit the number of liked tracks from SoundCloud, default: -1
         youtubePlaylistLimit: 20, // Limit the number of tracks in a YouTube playlist, default: -1
         spotifyPlaylistLimit: 30, // Limit the number of tracks in a Spotify playlist, default: -1
      },
   });
   ```

## 📚 Documentation

If you're using aoi.js, you may check [the documentation to learn more here](https://aoi.js.org/extensions/aoi.music/aoimusic-introduction).

Otherwise you can check [these autogenerated docs](https://aoijs.github.io/aoi.music/)
