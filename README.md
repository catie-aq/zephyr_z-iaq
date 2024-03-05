# Z_IAQ

Z_IAQ custom target for Zephyr OS.

## Usage
1. Add the Z_IAQ module to your manifest file
    - With the [6tron manifest](https://github.com/catie-aq/zephyr_6tron-manifest):
    ```bash
        - name: 6tron-manifest
          remote: catie-6tron
          repo-path: zephyr_6tron-manifest
          revision: main
          path: 6tron/6tron-manifest
            name-blocklist:
              - z-iaq
    ```
    - Without the [6tron manifest](https://github.com/catie-aq/zephyr_6tron-manifest):
    ```bash
        - name: 6tron-manifest
          remote: catie-6tron
          repo-path: zephyr_6tron-manifest
          revision: main
    ```

2. Compile your application for the Z_IAQ board
```bash
west build -b z_iaq <zephyr>/samples/hello_world
```

3. Flash your application
```bash
west flash
```
