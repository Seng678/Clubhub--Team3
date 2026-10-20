# Failure case analysis · Northeast Blackout of 2003 (v1.0, 2026-10-20)
Authors: Sinath Naihouy (Context & Timeline)

## 1. Context
On August 14, 2003, a massive cascading electrical blackout struck the Northeastern and Midwestern United States and Ontario, Canada, affecting 55 million people and shutting down over 100 power plants. The operational hub at the center of the initial failure was FirstEnergy Corporation, an Ohio-based electric utility. FirstEnergy relied on an Energy Management System (EMS) supplied by General Electric (GE)—specifically software known as XA/21—to monitor grid telemetry, process alarm states, and alert operators to dangerous overloads. The system mattered critically because human operators depended on its real-time visual and audio feedback to manage physical transmission lines and prevent localized failures from cascading across international borders.

## 2. Timeline
| Date | Event |
|------|-------|
| Aug 14, 2003 - 12:15 p.m. | Incorrect telemetry data renders a key state-estimator tool inoperative at MISO; operators fail to restart it. |
| Aug 14, 2003 - 2:02 p.m. | FirstEnergy’s 345 kV transmission line in Walton Hills, Ohio, sags and trips offline after contacting an overgrown tree. |
| Aug 14, 2003 - 2:14 p.m. | A race-condition bug in GE's XA/21 alarm subsystem freezes the primary alarm server silently, halting visual alerts. |
| Aug 14, 2003 - 3:05 p.m. | Additional overloaded FirstEnergy lines sag and trip into trees; control room operators remain unaware due to frozen alarms. |
| Aug 14, 2003 - 4:10 p.m. | A massive power surge flows through Michigan and Ontario, triggering automated safety breakers across regional grids. |
| Aug 14, 2003 - 4:13 p.m. | Over 100 power plants shut down automatically to protect equipment, plunging the entire region into a total blackout. |