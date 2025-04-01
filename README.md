import React from "react";

const TwitchLive = () => {
  const twitchUsername = "YOUR_TWITCH_USERNAME"; // Replace with your Twitch username
  const websiteDomain = "YOUR_WEBSITE.com"; // Replace with your website domain

  return (
    <div className="flex flex-col items-center justify-center min-h-screen bg-gray-900 text-white">
      <h1 className="text-3xl font-bold mb-4">Live Stream</h1>
      <div className="flex flex-col md:flex-row gap-4">
        {/* Twitch Player */}
        <iframe
          src={`https://player.twitch.tv/?channel=${twitchUsername}&parent=${websiteDomain}`}
          height="500"
          width="800"
          allowFullScreen
          className="rounded-lg shadow-lg"
        ></iframe>
        
        {/* Twitch Chat */}
        <iframe
          src={`https://www.twitch.tv/embed/${twitchUsername}/chat?parent=${websiteDomain}`}
          height="500"
          width="350"
          className="rounded-lg shadow-lg"
        ></iframe>
      </div>
    </div>
  );
};

export default TwitchLive;
