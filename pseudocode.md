# **Pseudocode Project**

## Gas Fireplace

<br>

<p><img src = './img/fire.jpg' alt = 'Gas Fireplace' width = '150' /></p>

### **Operational Expectations**:

The end-user will be able to turn the fireplace on or off at any desired time or set the unit to operate based on the desired room temperature. The fireplace controls are manual or remote via wireless remote control.

<hr>
<br>
<br>

# **Important Items**

<br>

- If the pilot light goes out, a device must be installed to automatically shut off gas flow to protect the end user from harm.

- The thermostat must have a conversion option so the unit will work in multiple markets. (Fahrenheit / Celsius)

- A safe, high-temperature setting must be set so an end-user cannot accidentally set the temperature above the recommended temperature setting for the fireplace specifications.

- A manual igniter system to ensure the pilot light cannot be lit remotely, ensuring the fireplace has been inspected before the first use of the season.

  <br>
  <br>

# **Object List**

- **End User**

- **Propane/Natural Gas Tank**
  - Gas Tank Valve
  - Gas line fittings

<br>

- **Gas Line**

  - Manual Burner Gas Valve
  - Gas line fittings

<br>

- **Gas Fireplace**

  - Fireplace Insert
  - Gas Burner
  - Decorative Log
  - Rock Wool
  - Control Unit
    - Three Way Switch
    - Flame Control Knob
    - Pilot light Control Feature (Flame Control Knob[PUSH IN])
    - Electronic Controlled Gas Valve
    - Remote Infrared/Bluetooth Sensor
  - Pilot light
  - Igniter
    - Igniter Button
  - Thermocouple
    <br/><br/>

- Wireless Remote Object
  - Digital display
  - Thermostat
  - Buttons
    - On button
    - Off button
    - Mode button
    - Batteries
      <br/><br/>

# **Objects, Functions, & Dependencies**

- ### **Gas Tank object**:

  - Purchased and provided by the end-user.

  - Gas Tank Object STORES gas for Gas Fireplace object.

  - Gas Tank Object CONNECTS to Gas Line Object with Gas Line Fitting.

    <br/><br/>

- ### **Manual gas valve**:

  - Part of the Gas Tank Object (Purchased by end-user)

    - **FUNCTION**: CONTROLS the flow of gas from the Gas Tank Object to Gas Line Object.

      - IF end-user TURNS Manual Gas Tank valve to the right

      - THEN gas WILL NOT flow.

      - IF end-user TURNS Manual Gas Tank valve to the left

      - THEN gas WILL flow.

<br/><br/>

- ### **Gas Line Object**:

  - Purchased by end-user and installed by licensed professional.

  - SUPPLIES gas from Gas Tank Object to Gas Fireplace Object.

  - Gas Line Object CONNECTS to Gas Burner Object with Gas Line Fitting.

    <br/><br/>

- ### **Manual Burner Gas valve**:

  - Purchased by end-user and installed by licensed professional.

    - **FUNCTION**: CONTROLS the flow of gas from Gas line Object to Gas Burner Object.

      - IF end-user TURNS Manual Burner Gas valve to right

      - THEN gas WILL NOT flow.

      - IF end-user TURNS Manual Burner Gas valve to left

      - THEN gas WILL flow.

    <br/><br/>

- ### **Gas Fireplace Object**:

  - Main object containing sub-components working together to operate as one object.

  - #### **Fireplace Insert Object**:

    - A metal frame mounted inside a wall to safely house Gas Fireplace Object.

    <br/><br/>

  - ### **Control Unit Object**:

    - Three Way Switch Object:

      - CONNECTS to electric power.

      - **FUNCTION**: CONTROLS electric power to the Control Unit Object.

        - IF switch is set to OFF

        - THEN no electric power to Control Unit Object.

        - IF switch is set to REMOTE AND Wireless Remote Object On Button NOT CLICKED

        - THEN no electric power to Control Unit Object.

        - IF switch is set to REMOTE AND Wireless Remote Object On Button CLICKED

        - THEN electric power SENT to Control Unit Object.

        - IF switch set to ON

        - THEN electric power to Control Unit Object.

    - Remote Infrared/Bluetooth Sensor Object:

      - **FUNCTION**: RECEIVES wireless signals from the Wireless Remote Object to remotely ACCESS the Control Unit Object.

        - IF Remote Sensor HAS electric power (IF infrared add AND sensor is not COVERED)

        - THEN Remote Sensor can receive Wireless Remote signal

        - IF Remote Sensor DOES NOT HAVE electric power (IF infrared add OR sensor is COVERED)

        - THEN Remote Sensor cannot receive Wireless Remote signal

    - **FUNCTION**: CONTROLS the volume of the flame produced by the Gas Burner Object.

      - Flame Control Knob Object provides a minimum and maximum amount the flame can be adjusted.

        - IF Flame Control Knob is LESS THAN 50%

        - THEN Gas Burner Object will produce flame LESS THAN 50% capacity.

        - IF Flame Control Knob is GREATER THAN 50% THEN

        - Gas Burner Object will produce flame GREATER THAN 50% capacity.

    - **FUNCTION**: CONTROLS the flow of gas from Gas Line Object to Gas Burner Object AND Pilot Light Object, by manually holding open the Electronic Controlled Gas Valve.

      - IF end-user PUSHES Flame Control Knob in

      - THEN Electronic Gas Valve manually opens ALLOWING gas to flow to Pilot Light Object.

<br/><br/>

- ### **The Igniter Object**:

  - ATTACHES to Gas Burner Object AND CONNECTS to electric power.

  - **FUNCTION**: PRODUCES an electric spark.

  - IF electric is CONNECTED AND end-user PUSHES Igniter Button

  - THEN Igniter Object will produce an electric spark.

<br/><br/>

- ### **Pilot light Object**:

  - ATTACHES to the Gas Burner Object next to the Igniter Object.

  - **FUNCTION**: PRODUCES continuous small flame to prevent unburnt gas from entering the living area and ease of lighting when desired.

    - To light Pilot Light Object USE Flame Control Object PUSH FUNCTION AND Igniter Object FUNCTION SIMULTANEOUSLY.

<br/><br/>

- ### **Thermocouple Object**:

  - ATTACHES to the Pilot Light Object directly above the flame.

  - **FUNCTION**: MEASURES temperature output of the Pilot Light Object and produces electric continuity in the circuit based on that output with the Electronic Controlled Gas Valve.

    - IF Thermocouple Object MEASURES temperature GREATER THAN specified temperature

    - THEN electric continuity is positive in the circuit with the Electronic Controlled Gas Valve.

    - IF Thermocouple Object MEASURES temperature LESS THAN specified temperature

    - THEN NO electric continuity in circuit.

<br/><br/>

- ### **Electronic Controlled Gas Valve Object**:

  - Part of the Control Unit Object (internal component), must connect to electric power.

  - **FUNCTION**: CONTROLS the flow of gas from the Gas Line Object to the Pilot Light Object and the Gas Burner Object.

    - To manually operate for temporary gas flow use the Flow Control Knob Object PUSH FUNCTION.

    - For valve to stay open it must receive an electric signal from the Thermocouple FUNCTION

  - **FUNCTION**: ALLOW gas glow if power failure.

    - IF Pilot Light Object is lit AND Electronic Controlled Gas Valve Object receives continuity from Thermocouple Object

    - THEN gas WILL flow to Gas Burner Object.

<br/><br/>

- #### **Gas Burner Object**:

  - Sits in the bottom of the Fireplace Insert Object.

  - Decorative Log Object SITS on top of Gas Burner Object to provide the look of an authentic fire.

  - Rock Wool Object SITS in the front bottom of the Fireplace Insert Object AND on top of the Gas Burner Object to provide the appearance of glowing embers.

  - **FUNCTION**: GENERATE flame from burning gas. - CONNECTS to: - Pilot Light Object - Thermocouple Object - Igniter Object - Control Unit Object - Gas Line Object - Remote infrared/Bluetooth Sensor Object
    <br/><br/>

### **Wireless Remote Object**:

- NOTE: Two (2) triple A batteries should be shipped with unit, however, all additional should be responsibility of end-user.
  <br/><br/>
- ### **Digital Display Object**:

  - **FUNCTION**: DISPLAYS the following

    - IF Gas Fireplace Object is on

    - THEN DISPLAY 🔥

    - IF Wireless Remote Object HAS power

    - THEN DISPLAY current room temperature

    - IF Wireless Remote Object is set to thermostat mode

    - THEN DISPLAY the word ROOM

    - IF Gas Fireplace Object is on AND set to manual mode

    - THEN DISPLAY the word TEMP

    - IF On Button is PUSHED on Wireless Remote Object

    - THEN DISPLAY the word ON

    - IF Off Button is PUSHED on Wireless Remote Object

    - THEN DISPLAY the word OF

    <br/><br/>

- ### **Thermostat**:

  - **FUNCTION**: CONTROLS the room temperature by turning the Gas Fireplace Object on if the room temperature drops below a certain temperature or off if it reaches a certain temperature.

  - A desired room temperature will need to be set

    - IF room temperature is LESS THAN desired temperature
    - THEN TURN ON Gas Fireplace Object
      - UPDATE Digital display object with current temperature, AND add 🔥 icon
    - IF room temperature is GREATER THAN desired temperature

    - THEN TURN OFF Gas Fireplace Object
      - UPDATE Digital display object with current temperature, AND remove 🔥 icon

  - **FUNCTION**: temperature CONVERSION from Fahrenheit to Celsius.

  - IF end-user PUSHES On Button Object AND Off Button Object simultaneously

  - THEN covert Fahrenheit temperature to Celsius temperature
    - UPDATE Digital display object with current temperature in Celsius

<br/><br/>

- ### **Buttons**:

  - ### **On Button**:

  - **FUNCTION**: SENDS wireless signal to Remote Infrared/Bluetooth Sensor Object to turn the Gas Burner Unit on.

    - IF Wireless Remote Object has battery power AND end-user PUSHES On Button

    - THEN the signal to turn on Gas Burner Object will be sent to Remote Infrared/Bluetooth Sensor Object
      - UPDATE Digital display object by ADDING 🔥

- ### **Off Button**:

  - **FUNCTION**: SENDS wireless signal toRemote Infrared/Bluetooth Sensor Object to turn the Gas Burner Unit off.

    - IF Wireless Remote Object has battery power AND end-user PUSHES Off Button

    - THEN the signal to turn off Gas Burner Object will be sent to Remote Infrared/Bluetooth Sensor Object
      - UPDATE Digital display object by REMOVING 🔥

- ### **Mode Button**:

  - **FUNCTION**:SWITCH between manual and thermostat operation of the Gas Fireplace Object.

  - Default state is manual mode.

    - IF Wireless Remote Object has battery power AND end-user PUSHES Mode Button

    - THEN signal sent to Remote Infrared/Bluetooth Sensor Object to switch current state

- ### **Set Button**:

  - **FUNCTION**: SETS the thermostat for the in the Wireless Remote Object which controls the Gas Fireplace Object.

    - IF Wireless Remote Object has battery power AND end-user PUSHES AND HOLDS Set Button until desired temperature is displayed (Digital Display Object will dynamical update until desired temperature is reached) AND end-user RELEASES Set Button

      - Wireless Remote Object will TIMEOUT for 3 seconds to store setting

    - THEN Thermostat Object is set

    - IF end-user goes past desired temperature CONTINUE hold Set Button until Digital Display Object reaches 99

    - THEN Digital Display will reset to 43

<br/><br/>

# **Gas Fireplace Object**

- **LIST OF FUNCTIONS NEEDED TO INITIALIZE OBJECT**:

- Manual Gas Valve Function (Gas Tank Object)
- Manual Burner Gas Valve Function (Gas Burner Object)
- Three Way Switch Function Remote OR On (Three Way Switch Object)
- Igniter Object Function _if Pilot Light Object not lit_ (Igniter Object)
- Pilot Light Function (Pilot Light Object)
- Thermocouple Function (Thermocouple Object)
- Electronic Controlled Gas Valve Function receiving continuity signal (Electronic Controlled Gas Valve)
- Gas Burner Function (Gas Burner Object)
