# ahb3lite_apb_bridge
Fully Parameterised Asynchronous AHB3-Lite to APB Bridge.

## Functionality
This IP contains 2 interfaces; an AHB3-Lite Slave interface and an APB Master interface. Any transactions received on the AHB Slave interface are translated into APB transactions on the APB master interface. If the APB datawidth is less than the AHB datawidth, then the core automatically generates APB burst transactions.
The interfaces can be on separate clock domains. The Bridge handles the clock domain crossing.

Notes:
- APB clock frequency must be equal or less than AHB clock frequency
- APB Datawidth must be equal or less than AHB data width
- APB and AHB datawidths must be multiples of bytes

## Documentation
[Datasheet](DATASHEET.md)

## Interfaces
- AHB3-Lite slave interface
- APB master interface

## Dependencies
This release requires the ahb3lite package found here https://github.com/RoaLogic/ahb3lite_pkg
