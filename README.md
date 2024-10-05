# FlyingStoneClone-01
Gnuk-compatible GnuPG USB Token

## Reasons for starting this project

Because I lost my old GPG key's password and need a better way to carry GPG key with me.

Hardware key + paperkey seems like a better solution, and luckily I met with Niibe Yutaka, who made a open-source GPG USB key project called Gnuk Token. 

## Design Considerations

- STM32F103CBT6 is more hand-soldering friendly
- ST-Link v2 can be used as testing platform
- If the hardware looks more like a ST-Link than a some mystical USB stick, it may have some "camouflage" for that
- Maybe I can use those left board as a ST-Link...
- Possibility of adding a ACK button

## Difference from FlyingStone-01/FlyingStone-01-G/FlyingStone-01-ShenZhen

FST-01:
- STM32F103TB, 12MHz XTAL
- PA2,PA3 exposed

FST-01G:
- Using the same MCU/XTAL as FST-01

FST-01SZ:
- GD32F103TB, 12MHz XTAL
- PA3 exposed by using a hall effect sensor (DRV5032FA)

FSC-01:
- STM32F103CB, 8MHz XTAL
- PA5,PB0,PB13,PB14,PA2,PA3 exposed, in which PA5 is designed to be used as ACK button

## What need to be done next

- test if Gnuk is function correctly
- test if NeuG is working
- test ESD safety
- test if this board can be used as ST-Link v2
