# FP2800a
Schematic symbol for KiCad of the FP2800a IC.

## Pinout of the FP2800a (top view):
```
                    ┌────┐ ┌────┐
            COM  x──┤1   └─┘  40├──o  2D
             1D  o──┤2        39├──o  2F
             1F  o──┤3        38├──o  2C
             1C  o──┤4        37├──o  2B
             1B  o──┤5        36├──o  2A
             1A  o──┤6        35├──►  VS
            GND ·|──┤7        34├──o  2E
             1E  o──┤8    F   33├──o  2G
             1G  o──┤9    P   32├──o  3G
             0G  o──┤10   2   31├──o  3E
             0E  o──┤11   8   30├──o  3F
             0F  o──┤12   0   29├──o  3D
             0D  o──┤13   0   28├──o  3C
             0C  o──┤14   a   27├──o  3B
             0B  o──┤15       26├──o  3A
             0A  o──┤16       25├──|· GND
            VCC  ◄──┤17       24├──<  ENABLE
             A1  >──┤18       23├──<  DATA
             A0  >──┤19       22├──<  B1
             A2  >──┤20       21├──<  BO
                    └───────────┘
```

## Symbol Legend:
```
  ├──o  IO
  ├──<  Input
  ├──>  Output
  ├──►  Positiv Voltage
  ├──|· Ground
  ├──x  unused
```

## Description for IO, Input and Output pins
* A0-A2 and B0-B1: control inputs to select which of the usable IO pins should be activated
* 0A-3G: usable IO pins to sink or source current
* DATA: change selected IO type to between sink if low or source if high
* ENABLE: activates the selected IO while kept high

## Further details
Source code to control this chip can be found within the project [Flip-The-Dot](https://github.com/RobsyRocket/Flip-The-Dot).
