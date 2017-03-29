# ahb3lite_apb_bridge
Fully Parameterised Asynchronous AHB3-Lite to APB Bridge.

<h2>Functionality</h2>
This IP contains 2 interfaces; an AHB3-Lite Slave interface and an APB Master interface. Any transactions received on the AHB Slave interface are translated into APB transactions on the APB master interface. If the APB datawidth is less than the AHB datawidth, then the core automatically generates APB burst transactions.
The interfaces can be on separate clock domains. The Bridge handles the clock domain crossing.

Notes:
- APB clock frequency must be equal or less than AHB clock frequency
- APB Datawidth must be equal or less than AHB data width
- APB and AHB datawidths must be multiples of bytes

<h2>Interfaces</h2>
- AHB3-Lite slave interface
- APB master interface

<h2>Dependencies</h2>
This release requires the ahb3lite package found here https://github.com/RoaLogic/AMBA/tree/master/AHB/ahb3lite_pkg
