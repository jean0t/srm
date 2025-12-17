# Safe Remove (SRM)

**Safe Remove (SRM)** is a simple and efficient Linux utility designed to securely delete files.
Instead of merely unlinking a file from the filesystem, SRM overwrites its contents multiple times before removal, significantly reducing the chance of data recovery.

The goal of SRM is to provide **privacy, safety, and ease of use**, while keeping the interface familiar to anyone who already uses `rm`.

---

## Features

* Secure file deletion by overwriting file contents multiple times
* Simple and lightweight
* Designed to behave like the standard `rm` command
* Supports the same command-line options as `rm`
* Ideal for users who value privacy and data safety

---

## Installation

Installation is straightforward and requires no build process.

1. Copy the script to `/usr/local/bin`:

   ```sh
   sudo cp srm /usr/local/bin/
   ```

2. Make it executable:

   ```sh
   sudo chmod u+x /usr/local/bin/srm
   ```

After that, `srm` will be available system-wide like any other command.

---

## Usage

SRM is intended to be as practical and intuitive as `rm`.

Basic usage:

```sh
srm file.txt
```

You can use it directly from the terminal with the same options you would normally use with `rm`.

Example:

```sh
srm -v important_file.txt
```

This design allows you to replace `rm` with `srm` in your workflow with minimal friction.

---

## Limitations

* **Directory removal is not supported yet**

Support for directories is planned for the next update.

---

## Roadmap

* Add secure directory removal
* Improve overwrite strategies and configurability
* Additional safety checks

---

## Disclaimer

While SRM significantly reduces the chances of file recovery, no software-based solution can guarantee absolute irrecoverability on all storage devices (especially SSDs with wear leveling). Use responsibly and understand your storage medium.

---

## License

GPL-3
