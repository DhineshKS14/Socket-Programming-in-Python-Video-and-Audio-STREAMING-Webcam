# vidstream

Under construction! Not ready for use yet! Currently experimenting and planning!

Developed by Florian Dedov from NeuralNine (c) 2020

## Examples of How To Use (Buggy Alpha Version)

Creating A Server

```python
from vidstream import StreamingServer

server = StreamingServer('127.0.0.1', 9999)
server.start_server()

# Other Code

# When You Are Done
server.stop_server()
```

Creating A Client
```python
from vidstream import CameraClient
from vidstream import VideoClient
from vidstream import ScreenShareClient

# Choose One
client1 = CameraClient('127.0.0.1', 9999)
client2 = VideoClient('127.0.0.1', 9999, 'video.mp4')
client3 = ScreenShareClient('127.0.0.1', 9999)

client1.start_stream()
client2.start_stream()
client3.start_stream()
```

Check out: https://www.youtube.com/c/NeuralNine

Sure! Here’s a basic structure for a GitHub README file for your project:

---

# Video and Audio Streaming with TCP Socket Programming

## Overview

This project demonstrates video and audio streaming using socket programming in Python. By utilizing Transmission Control Protocol (TCP), the project ensures reliable communication between client and server. TCP's three-way handshake and its ability to handle packet loss and ordering are leveraged to provide a robust streaming solution.

## Features

- **Video and Audio Transmission**: Stream video and audio data from a server to a client.
- **Reliable Communication**: TCP ensures that data is transmitted correctly, handling packet loss and maintaining order.
- **User Interface**: Built using Tkinter for the client-side interface.
- **Video Processing**: Utilizes OpenCV for video capture and processing.

## Technologies Used

- **Python**: Programming language used for implementation.
- **TCP**: Transmission Control Protocol for reliable data transmission.
- **OpenCV**: Library used for video processing and capture.
- **Tkinter**: Library used for creating the client-side graphical user interface (GUI).

## Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/yourusername/your-repository.git
   cd your-repository
   ```

2. **Install the required libraries:**

   Make sure you have Python installed, then install the required packages:

   ```bash
   pip install opencv-python tkinter
   ```

## Usage

1. **Run the Server:**

   Navigate to the server directory and execute:

   ```bash
   python server.py
   ```

2. **Run the Client:**

   Navigate to the client directory and execute:

   ```bash
   python client.py
   ```

3. **Interact with the GUI:**

   The client application will launch a window where you can view the streamed video and interact with the audio features.

## Code Structure

- **`server.py`**: Contains the server-side code for handling video and audio streaming.
- **`client.py`**: Contains the client-side code for receiving and displaying video and audio streams.
- **`utils.py`**: Includes utility functions used by both server and client (e.g., data encoding/decoding).

## Key Concepts

- **TCP Three-Way Handshake**: A process used to establish a reliable connection between client and server.
- **Reliable Transmission**: Ensured by TCP, which handles packet loss and ordering issues.
- **Socket Programming**: Enables communication between two devices over a network.

## Contributing

Feel free to open issues, submit pull requests, or suggest improvements. Your contributions are welcome!

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgements

- [OpenCV](https://opencv.org/) for video processing.
- [Tkinter](https://docs.python.org/3/library/tkinter.html) for GUI development in Python.

---

Feel free to adjust any details based on your actual implementation and repository structure!
