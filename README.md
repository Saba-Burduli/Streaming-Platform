# 🎥 WebCam Streaming with ASP.NET Core

This is a simple proof-of-concept project demonstrating **webcam streaming** in **ASP.NET Core** web applications using:

- 🌐 `System.Net.WebSockets.WebSocket`
- ⚡️ `ASP.NET Core SignalR`
- 🚀 WebRTC *(Coming soon...)*

The project shows how webcam data can be streamed between clients and the server using different technologies — all for learning and fun! 😄

---

## 🔧 Features

### 1. WebSocket-based Streaming (Grayscale Filter)

- A **WebSocket** connection is established between the client and server.
- On the **client-side**, webcam video is captured and sent as JPEG frames.
- Frames are transmitted to the server at a controlled **FPS** to avoid glitches.
- The **server processes** each frame (e.g., applies a grayscale filter).
- Processed frames are returned to the client as **Base64 image strings** and displayed in real-time.

🎯 This demonstrates how client-side streams can be processed server-side for effects or analysis.

---

### 2. SignalR-based Peer-to-Peer Streaming

- Two clients connect to the same ASP.NET Core app (Razor-based frontend).
- **Client-A** initiates a video call to **Client-B**.
- **Client-B** gets a **call notification** and can **accept or decline** the call.
- Once accepted:
  - A SignalR **Hub** connection is established between both clients.
  - **Client-A’s webcam** stream is sent to the server.
  - The server **relays the stream** to **Client-B** using SignalR’s standard client method calls.

🎯 This demonstrates a simple **peer-to-peer-like** interaction using SignalR without WebRTC.

---

## 🚧 Coming Soon

- ✅ **WebRTC** integration for true P2P media streaming (no server relaying).
- 🎛️ UI Improvements & Better Controls
- 🎨 Filters & Effects
- 🔒 Authentication & Access Control

---

## 📚 References & Useful Links

- [Use streaming in ASP.NET Core SignalR](https://learn.microsoft.com/en-us/aspnet/core/signalr/streaming)
- [WebSockets support in ASP.NET Core](https://learn.microsoft.com/en-us/aspnet/core/fundamentals/websockets)

---

## 🧪 Notes

This project was built over a weekend just to explore what's possible in ASP.NET Core when it comes to **real-time webcam streaming**. It was fun to build, and I’m happy with the results — so here’s the repo! 😄

---

## 🛠️ Technologies Used

- ASP.NET Core
- Razor Pages
- JavaScript
- WebSockets
- SignalR
- HTML5 `<video>` and `<canvas>` APIs

---

## 🚀 Run & Try

> Instructions on how to build and run this project locally will be added soon...

---

## 🤝 Contributions

Pull requests, ideas, and improvements are welcome!

---

## 📄 License

MIT – Do whatever you want, just have fun 😎


