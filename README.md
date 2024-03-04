# Java Webserver

This project is a simple implementation of a web server using socket programming in Java.The primary goal of this project is to compare the performance differences between single-threaded, multi-threaded, and thread pool implementations. The server accepts or rejects client connections and measures latency.

## Table of Contents

- [Folder Structure](#folder-structure)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Folder Structure

The project is organized into the following folders, each containing a different implementation of the web server:

- **single-threaded**: Contains the source code for a single-threaded implementation of the web server.
  - `SingleThreadedWebServer.java`: Main server file.
  - `SingleThreadedWebClient.java`: Client file for testing.

- **multi-threaded**: Contains the source code for a multi-threaded implementation of the web server.
  - `MultiThreadedWebServer.java`: Main server file.
  - `MultiThreadedWebClient.java`: Client file for testing.

- **thread-pool**: Contains the source code for a thread pool implementation of the web server.
  - `ThreadPoolWebServer.java`: Main server file.
  
## Features

- Basic HTTP server functionality.
- Implements different threading strategies (single-threaded, multi-threaded, thread pool) for handling client requests.

## Installation

To run the Java Webserver, you will need to have Java Development Kit (JDK) installed on your system.

1. Clone this repository:

```bash
git clone https://github.com/gopikrishna152/WebServer.git



## Usage 

Each implementation of the web server can be run separately. Follow the instructions in the respective folder to compile and run the server:
javac *.java

java Server

## Testing TCP Functionality

### Setting up JMeter for TCP Testing:

1. **Download and Install JMeter**: If you haven't already, download and install Apache JMeter from the official website.

2. **Add TCP Sampler**: In JMeter, TCP samplers are used to send TCP requests. You can add TCP Sampler by right-clicking on the Thread Group → Add → Sampler → TCP Sampler.

3. **Configure TCP Sampler**:
   - Provide the server name or IP address and port number of the TCP server you want to test.
   - Choose the desired request and response format (e.g., text, binary).
   - Set any required timeout values.

4. **Add Listeners**: Listeners in JMeter are used to view test results. You can add listeners to see the responses received from the TCP server. Common listeners for TCP testing include View Results Tree, View Results in Table, or Summary Report.

### Testing Steps:

1. **Thread Group Configuration**: Configure the Thread Group with the desired number of threads (users) and loop count (iterations).

2. **Configure TCP Sampler**: Set up the TCP Sampler with the necessary server details and request data.

3. **Add Assertions (Optional)**: You can add assertions to validate the response received from the server. Assertions help ensure that the response meets specific criteria.

4. **Run the Test**: Click on the "Start" button to run the test plan.

5. **View Results**: After the test completes, analyze the results using the configured listeners. Pay attention to response times, error rates, and any issues encountered during the test.

### Tips for TCP Testing with JMeter:

- **Keep it Simple**: TCP testing in JMeter can be straightforward, especially for simple request-response interactions. Start with basic configurations and gradually add complexity as needed.

- **Use Assertions**: Assertions help verify the correctness of responses. Use them to ensure that the server is returning the expected data.

- **Consider Connection Pools**: If your TCP server uses connection pooling or persistent connections, ensure that your test plan reflects this behavior to simulate real-world scenarios accurately.

- **Monitor Resource Usage**: Testing TCP protocols may consume significant resources, especially with high loads. Monitor CPU, memory, and network usage on both the JMeter machine and the server under test.

- **Debugging**: Use JMeter's Debug Sampler and Debug PostProcessor to troubleshoot any issues encountered during testing.

- **Security**: If you're testing secure TCP protocols (e.g., SSL/TLS), ensure that you configure JMeter appropriately with the necessary certificates and security settings.





This updated README.md file provides a brief overview of the folder structure and contents of the project, including descriptions of each implementation of the web server along with their respective client and server source code files. 


