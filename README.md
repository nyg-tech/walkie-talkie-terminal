# 📟 walkie-talkie-terminal

A browser-to-browser (WebRTC) **push-to-talk (PTT)** walkie-talkie app with a retro terminal theme. No server, no signup — hold the button, talk, release.

---

## ✨ Features

- **Push-to-talk (PTT):** Hold the button to talk, release to go silent — just like a real walkie-talkie.
- **Create or join a channel:** Spin up a room instantly with a 5-character channel code, or join an existing one.
- **Admin-approved entry:** Whoever opens the channel automatically becomes the **admin** 👑. Anyone requesting to join first lands in the admin's approval queue — the admin **accepts** or **rejects**.
- **Live participant list:** See who's connected and who's currently transmitting, with a live LED indicator.
- **Flag picker:** Choose a country flag for yourself from the settings menu; it shows up next to your name in the participant list.
- **Multi-language:** Turkish / English — switch instantly from the settings menu.
- **Serverless audio:** Audio streams directly browser-to-browser (WebRTC/PeerJS); a public PeerJS server is only used for connection setup (signaling). No audio is ever recorded or stored server-side.
- **Single file:** No build step, no install. Just open one `.html` file.



## 🛠️ Tech

- Pure HTML/CSS/JavaScript — no build tools or frameworks.
- Uses [PeerJS](https://peerjs.com/) (a WebRTC wrapper) for audio and data connections.
- Signaling (connection setup) relies on PeerJS's public cloud server by default; you can point it at your own PeerJS server instead.


```

## 🔒 Privacy

- Audio traffic flows peer-to-peer directly between participants and is never stored on a server.
- Callsign, flag, and room info live only in memory for the duration of the session; nothing is persisted anywhere.

