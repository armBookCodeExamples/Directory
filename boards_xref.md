# Board Cross-references

| Board          | Device (Rev)     | Core       | Reference Manual | Board design | Reference Manual | Equivalencies<sup>1</sup> |
|----------------|------------------|------------|------------------|--------------|------------------|---------------------------------|
| [NUCLEO-F429ZI](https://os.mbed.com/platforms/ST-Nucleo-F429ZI/)  | [STM32F429ZIT6](https://www.st.com/resource/en/datasheet/stm32f429zi.pdf) | Cortex-M4  |[RM0090](https://www.st.com/resource/en/reference_manual/dm00031020-stm32f405-415-stm32f407-417-stm32f427-437-and-stm32f429-439-advanced-arm-based-32-bit-mcus-stmicroelectronics.pdf) | [MB1137](https://www.st.com/resource/en/schematic_pack/nucleo_144pins_sch.zip) |[UM1974](https://www.st.com/resource/en/user_manual/um1974-stm32-nucleo144-boards-mb1137-stmicroelectronics.pdf) |NUCLEO-F207ZG, NUCLEO-F303ZE, NUCLEO-F412ZG, NUCLEO-F413ZH, NUCLEO-F429ZI, NUCLEO-F439ZI, NUCLEO-F446ZE, NUCLEO-F722ZE, `NUCLEO-F746ZG`, NUCLEO-F756ZG, NUCLEO-F767ZI and NUCLEO-H743ZI |
| [NUCLEO-F746ZG](https://os.mbed.com/platforms/ST-Nucleo-F746ZG/)  | [STM32F746ZGT6](https://www.st.com/resource/en/datasheet/stm32f746zg.pdf) | Cortex-M7  | [RM0385](https://www.st.com/resource/en/reference_manual/rm0385-stm32f75xxx-and-stm32f74xxx-advanced-armbased-32bit-mcus-stmicroelectronics.pdf) | MB1137 | UM1974 | ^^^ |
| [NUCLEO-F401RE](https://os.mbed.com/platforms/ST-Nucleo-F401RE/)  | [STM32F401RE](https://www.st.com/resource/en/datasheet/stm32f401re.pdf) | Cortex-M4  | [RM0368](https://www.st.com/resource/en/reference_manual/rm0368-stm32f401xbc-and-stm32f401xde-advanced-armbased-32bit-mcus-stmicroelectronics.pdf) | [MB1136](https://www.st.com/resource/en/schematic_pack/mb1136-default-c04_schematic.pdf) | [UM1724](https://www.st.com/resource/en/user_manual/um1724-stm32-nucleo64-boards-mb1136-stmicroelectronics.pdf) | NUCLEO-F030R8, NUCLEO-F070RB, NUCLEO-F072RB, NUCLEO-F091RC, NUCLEO-F103RB, NUCLEO-F302R8, NUCLEO-F303RE, NUCLEO-F334R8, NUCLEO-F401RE, NUCLEO-F410RB, NUCLEO-F411RE, NUCLEO-F446RE, NUCLEO-L010RB, NUCLEO-L053R8, NUCLEO-L073RZ, NUCLEO-L152RE , NUCLEO-L452RE, NUCLEO-L476RG |

[1]: "Equivalencies": same pinout, but _not necessarily_ same peripherals in those pins, nor same way to configure them

## LEDs + Push-buttons

| Board          | LED1  | LED2 | LED3 | Push-button |
|----------------|-------|------|------|-------------|
| NUCLEO-F429ZI  |6.5: LD1, green, PB0, active high | 6.5: LD2, blue, PB7, active high | 6.5: LD3, red, PB14, active high | 6.6: B1, PC13; schematic: **active high** |
| NUCLEO-F401RE  | :cry: | 6.4: LD2, green, shared with Arduino D13(Table 16): PA5 (Table 11 - Table 23), active high | :cry: | 6.5: B1, PC13; schematic: **active low**  |
