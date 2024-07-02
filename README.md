<h2># Simple HTTP Client in Rust with Error Handling</h2>
<p>This repository contains a simple Rust program that demonstrates making an HTTP GET request using the `reqwest` crate, and handling potential errors using the `error_chain` crate.</p>

<p>## Features</p>
<li> Makes a GET request to `http://httpbin.org/get`.</li>
<li> Handles HTTP request errors and IO errors gracefully.</li>
<li> Prints the status, headers, and body of the HTTP response.</li>
<br>

<p>## Prerequisites</p>
<li> [Rust](https://www.rust-lang.org/tools/install) (1.45.0 or later)</li>
<br>

<p>## Usage</p>

1. Clone the repository:

    ```sh
    git clone https://github.com/your-username/rust-http-client.git
    cd rust-http-client
    ```

2. Build the project:

    ```sh
    cargo build
    ```

3. Run the project:

    ```sh
    cargo run
    ```

<p>## Code Explanation</p>

<p>The code uses the `error_chain` crate to manage errors and the `reqwest` crate to perform HTTP requests.</p>
<p>### Dependencies</p>

<p>Add the following dependencies to your `Cargo.toml` file:</p>

```toml
[dependencies]
reqwest = { version = "0.11", features = ["blocking"] }
error-chain = "0.12.4"
