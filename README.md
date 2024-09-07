# PLC_WaterPumpControl_Codesys_FBD

PLC Water Pump Control System (FBD Simulation)

This project demonstrates a water pump control system using Function Block Diagram (FBD) programming in CODESYS. The system is designed to simulate water distribution control, operating in both manual and automatic modes, based on sensor input, valve status, manual inputs. (There are no actual PLCs or HMIs involved; the system is entirely simulated.)

---
-  System Components
    -  Sensors (Analog):
       - Hydrostatic Level Sensor: Measures water level inside the deposit.
       - Pressure Sensor: Monitors pump pressure.
    -  Manual Valves: There are three valves. If all are closed, no water is pumped. Valves are assumed to be manual.
    -  HMI giving manual start/stop and sytem operation mode select


-  Operating Modes <br>

   Automatic Mode : Starts system operation based on sensor inputs.
    -  All three valves must be open.
    -  Pump pressure must exceed 5 bars.
    -  Water level in the deposit must be above 2 meters.


-  Manual Mode : System operates with all three valves open, ignoring sensor readings.
    

-  Safety Features
    The pump stops immediately if:
    - The emergency stop button is triggered.
    - An overload signal is detected.

---
PLC Simulation (Hypothetical) <br>
-  Digital Inputs :
   -  Valve 1 (1V)
   -  Valve 2 (2V)
   -  Valve 3 (3V)
   -  Emergency Stop
   -  Overload Signal

-  Digital Outputs :
    Controls a relay that activates a contactor, which starts the pump motor.

-  Analog Inputs :
    Simulated input readings from the Hydrostatic Level Sensor and Pressure Sensor.

HMI Control : 
   - Automatic/Manual Mode Selection
   - Manual Start Button
   - Manual Stop Button


FBD Program in CODESYS,
The core of this project is the Function Block Diagram (FBD), written and simulated in CODESYS to control the pump operation based on the specified conditions.
   
