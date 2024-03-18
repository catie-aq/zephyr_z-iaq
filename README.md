# Z_IAQ

[Z_IAQ](https://6tron.io/z_object/z_iaq) custom target for Zephyr OS.

## Supported Features

The Zephyr Z_IAQ board configuration supports the following hardware features:

| Interface | Controller                                                                                   | Driver/Component |
| :-------- | :------------------------------------------------------------------------------------------- | :--------------- |
| CLOCK     | on-chip                                                                                      | clock_control    |
| FLASH     | on-chip                                                                                      | flash            |
| GPIO      | on-chip                                                                                      | gpio             |
| I2C(M)    | on-chip                                                                                      | i2c              |
| MPU       | on-chip                                                                                      | arch/arm         |
| NVIC      | on-chip                                                                                      | arch/arm         |
| PWM       | on-chip                                                                                      | pwm              |
| RADIO     | on-chip                                                                                      | Bluetooth        |
| UART      | on-chip                                                                                      | serial           |
| WDT       | on-chip                                                                                      | watchdog         |
| SENSOR    | [BME688](https://www.bosch-sensortec.com/products/environmental-sensors/gas-sensors/bme688/) | Not supported    |

## Usage

1. Add `Z_IAQ` board to your workspace using the [6TRON module](https://github.com/catie-aq/zephyr_6tron-manifest.git)
2. Compile and flash application using west tool
   - Board name: `z_iaq`
