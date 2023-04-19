# HFT Execution Server

A High-Frequency Trading (HFT) execution server implemented in Rust, supporting Bybit and Binance 
cryptocurrency exchanges. The server is designed for low-latency, high-performance trading and is 
extensible to support additional exchanges, trading algorithms, and order types.

## Features

- Low-latency and high-performance order execution
- Support for Bybit and Binance exchanges
- WebSocket-based communication for real-time market data and order updates
- Built-in trading algorithms: Chase, TWAP, VWAP
- Order types: Market, Limit, Chase, TWAP, VWAP, and Basket orders
- Journaling functionality for recording trade data, order states, and algorithmic decisions
- Modular architecture and message-passing concurrency for easy extensibility and maintainability

## Getting Started

### Prerequisites

- [Rust](https://www.rust-lang.org/tools/install): Install the Rust programming language and its 
package manager, Cargo.
- API keys: Obtain API keys for the supported exchanges (Bybit and Binance) to enable trading.

### Installation

1. Clone the repository:

git clone https://github.com/yourusername/HFT-Execution-Server.git

2. Change to the project directory:
cd HFT-Execution-Server

cargo build --release


### Configuration

1. Create a configuration file named `config.toml` in the project root directory:

touch config.toml


2. Edit `config.toml` to include your exchange API keys and any other desired settings:

```toml
[bybit]
api_key = "your_bybit_api_key"
api_secret = "your_bybit_api_secret"

[binance]
api_key = "your_binance_api_key"
api_secret = "your_binance_api_secret"

Refer to the src/config/mod.rs file for additional configuration options.

Running the Server
Start the HFT execution server:
cargo run --release
Monitor the logs for any errors or important information.

Contributing
We welcome contributions to the HFT Execution Server project. Please follow these steps to 
contribute:

Fork the repository on GitHub.
Create a new branch for your changes.
Commit your changes and push them to your fork.
Create a pull request describing your changes and submit it to the main repository.
Please ensure your changes are well-documented and include appropriate tests.

Reporting Issues
If you encounter any issues or bugs while using the HFT Execution Server, please open an issue on the 
GitHub repository. Be sure to provide detailed information about the issue, including steps to 
reproduce the problem, the expected outcome, and any relevant logs or error messages.

Feature Requests
We welcome feature requests for the HFT Execution Server. To request a new feature, please open an 
issue on the GitHub repository and describe the desired functionality, its benefits, and any 
potential implementation challenges.

License
This project is licensed under the MIT License. See the LICENSE file for details.


