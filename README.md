## Request Prober Using Rust . 

Simple Rust Codes to Demonstrate Request and Response using Tokio Library and using various methods to Request and get the status code . 

Main Purpose is for testing when working with firewall while testing the black list.

## Features

- **Protocol Agnostic**: Automatically detects and checks both HTTP and HTTPS versions of URLs if the protocol is not specified.
- **Concurrent Processing**: Employs asynchronous tasks to concurrently check multiple URLs, enhancing speed and efficiency.
- **Color-Coded Output**: Utilizes color-coding to represent different response statuses for easy visualization.
- **Timeout Handling**: Manages timeouts effectively, indicating URLs that take too long to respond.

## How to Use

### Installation

1. **Clone the Repository**

```
git clone https://github.com/Whitecat18/Reqwest-Prober-Rust.git
cd Reqwest-Prober-Rust
```

2 . **To run the Program**

```
cargo run -- url_file.txt 
```
## Bug Fixes and Errors 

### For Debian Based Users Ubuntu/Kali 

<details>
  <summary><b>Detailed Error Info</b></summary>
  The Following Error Occures while testing on Kali Linux .<br>
  
  ```
  run pkg_config fail: 
  pkg-config exited with status code 1
  > PKG_CONFIG_ALLOW_SYSTEM_CFLAGS=1 pkg-config --libs --cflags openssl
  ```

</details>

If you face an openssl error install the following dependics and try again ! 



```
sudo apt install libssl-dev pkg-config libudev-dev
```

## Advantages

- **Efficiency**: Concurrent checking of URLs speeds up the process, especially when dealing with numerous URLs.
- **Ease of Use**: Simple command-line interface, requiring just a file path containing URLs.
- **Visual Clarity**: Color-coded output aids in quickly identifying the status of each URL.
