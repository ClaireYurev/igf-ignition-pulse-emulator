# IGF Ignition Pulse Emulator

This is a hardware prototype project that aims to emulate the return signal on 4-pin Toyota ignition coil systems, where the physical coil only utilizes the 3 pins actively.

In other words, while the connector provides 4 pins - most commonly found coils are missing the IGF signal. The coil simply doesn't produce this signal. The IGF signal is supposed to be produced by each coil as a positive confirmation for the vehicle ECU that the sparkplug has fired.

In systems where this IGF signal is not produced by the coil itself, it is possible to create a hardware emulator that will come close to replicating the true IGF signal.

The purpose of this is to allow the engine to run, as opposed to being immediately shut down by the ECU after starting (once the ECU detects that the IGF signal has not arrived for 6-8 engine ignition cycles). 