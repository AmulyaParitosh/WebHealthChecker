# WebHealthChecker

WebHealthChecker is a powerful command-line tool built in Go that allows you to quickly and easily check the status of a website. Whether you're a developer, system administrator, or just curious about a website's availability, WebHealthChecker provides a simple and efficient way to determine if a website is up and running.

[![Go](https://img.shields.io/badge/Go-00ADD8?style=for-the-badge&logo=go&logoColor=white)](https://go.dev/)
[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/AmulyaParitosh/WebHealthChecker)

## Table of Contents

- [Features](#features)
- [Installation](#installation)
  - [Pre-built Binaries](#pre-built-binaries)
  - [Building from Source](#building-from-source)
- [Usage](#usage)
- [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)

## Features

- Quick and easy website status checking
- Customizable port selection
- Cross-platform compatibility (Windows and Ubuntu)
- Simple command-line interface
- Lightweight and fast execution

## Installation

### Pre-built Binaries

For quick installation, you can download the pre-built binaries for your operating system:

#### Ubuntu
```bash
wget https://amulyaparitosh.github.io/WebHealthChecker/build/ubuntu/webcheck
chmod +x webcheck
sudo mv webcheck /usr/local/bin/
```

#### Windows
1. Download the executable from [this link](https://amulyaparitosh.github.io/WebHealthChecker/build/windows/webcheck.exe).
2. Add the directory containing `webcheck.exe` to your system's PATH environment variable.

### Building from Source

If you prefer to build the tool from source or want to contribute to its development, follow these steps:

1. Ensure you have Go installed on your system. If not, download and install it from [the official Go website](https://golang.org/dl/).

2. Clone the repository:
   ```bash
   git clone https://github.com/AmulyaParitosh/WebHealthChecker.git
   ```

3. Navigate to the project directory:
   ```bash
   cd WebHealthChecker
   ```

4. Build the project:
   ```bash
   go build -o webcheck .
   ```

   This will create an executable named `webcheck` in your current directory.

5. (Optional) Move the executable to a directory in your PATH for easy access:
   ```bash
   sudo mv webcheck /usr/local/bin/
   ```

## Usage

WebHealthChecker is designed to be simple and straightforward to use. Here's the general syntax:

```
WebHealthChecker [global options] command [command options]
```

### Global Options

- `--domain value, -d value`: Specify the domain name to check.
- `--port value, -p value`: Specify the port number to check.
- `--help, -h`: Show help information.

### Commands

- `help, h`: Shows a list of commands or help for one command.

## Examples

1. Check a website's status on the default port (80):
   ```bash
   webcheck -d example.com
   ```

2. Check a website's status on a specific port:
   ```bash
   webcheck -d example.com -p 8080
   ```

3. Display help information:
   ```bash
   webcheck --help
   ```

## Contributing

Contributions to WebHealthChecker are welcome! If you have suggestions for improvements or bug fixes, please feel free to:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
