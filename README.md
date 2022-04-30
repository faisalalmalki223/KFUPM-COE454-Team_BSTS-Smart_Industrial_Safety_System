# KFUPM-COE454-Team_BSTS-SISS
  As part of the COE 454 course, we formed our team to work on a course project.
  
## Team Name: Better Safe Than Sorry
  ### Our team is comprised of two members:
    1- Khalid Al-Shehri
    2- Faisal Al-Malki

## Project Title: Smart Industrial Safety System
  Our project idea is to create an IOT-powered industrial safety system with various use cases.
  We used Cisco Packet Tracer to create most of the system and the environment for the use cases,
  in addition to a python client that communicates with the aforementioned environment and system.

## Overview of functionality and organization:
  ### ◙SSS: Safety Shutdown System
    Use case: Shutdown certain machinery / zones to a safe state if an emergency is detected.
      • Help detect unauthorized personnel or employees that do not abide by safety distance 
        from machinery, disable machinery for the employee’s safety.
      • Allow employees to issue manual safety shutdown signal “manual kill-switch”.
      • Monitor excessive power use to indicate issues with machinery, or if a machine is stalled 
        due to a malfunction or if an employee is incapacitated by it.
 ### ◙FGS: Fire and gas system
    Use case: Detect toxic gases, fires, high temperatures. 
    • Send unusual levels to cloud for analysis and logging, cloud may decide to issue warning or 
      action signal
    • In emergencies, act accordingly locally by fire suppression systems, warning lights and 
      sirens.
    • Upon clearance of emergency, drain fire suppressant to help restore industrial zone back to 
      functional state.
    • Monitor temperature of sensitive zones and regulate it.
 ### ◙Sensors used:
    • Trip sensor, Motion sensor, Smoke sensor, Temperature sensor, Toggle Push button
 ### ◙Actuators:
    • Alarm, Ceiling and Floor sprinkler, Speakers, Motor (Ventilation Fan), Water Drain
 ### ◙Processing:
    ○ Edge 
     • In emergencies, act according to manual kill-switch button (SSS)
     • React to fires and gas locally by fire suppression modules, warning lights and sirens. (FGS)
    ○ Fog
     • Compare safety levels of zones and act upon choosing zones to be shutdown (SSS)
     • Monitor power consumption of zones to notice fluctuations and react accordingly (SSS)
     • Local zone temperature regulation (FGS)
    ○ Cloud
     • Analysis and logging of long term collected data from FGS, cloud may decide to issue 
     • warning or action signal to start fire suppression.
 ### ◙Visualization
     • Visualize FGS readings of each zone, visualize map running / disabled zones as result of SSS.
