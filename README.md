# Pogo Pin Connector

The pogo pin connector (PPC) board is used to help record the IR emissions of a solar cell when connected backwards. The board is first connect to the lines of the cell, current is injected from a power supply, and an IR camera captures the IR emissions from the cell. The PPC board is used on either side of the cell to provide a path for the current to flow. Before the PPC board, cells were tested by clamping two aluminum blocks to the exposed lines. This resulted in issues since some of the lines had better contact than others as was evident in the resulting IR image. The pogo pins are meant to apply even pressure and contact to all of the exposed lines and give a better IR image. 

![3d model](images/3d_model.png)

## Schematic

The following image is the schematic of the PPC board. The two mounting holes, H1 and H2, are size M3 and will screw in two ring terminals that connect to a power supply. There are then sixty pogo pins connected in series between the two mounting holes. 

![schematic](images/schematic.png)

## PCB Layout

The following images is the PCB layout of the PPC board. The two holes at the top are the ring connectors that supply power to the pogo pins. There are three mounting holes to connect the physical board to a jig. The panel is expected to draw around four amps so the trace is speced for six amps. Using the KiCad calculator for 2oz copper (70um thick), the trace needs to be ~1.8mm thick to be able to handle six amps. The rest of the board is filled with copper to provide better board thermals. The copper pour is not grounded but this is not expected to be an issue since the board is working with only DC supplies.

![pcb_layout](images/pcb_layout.png)
