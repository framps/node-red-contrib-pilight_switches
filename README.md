# node-red-contrib-pilight

[pilight](https://www.pilight.org/) supports various 433MHz devices. This node should help to use 433MHz switches via pilight in Node-Red.

## Note
This custom node is still not final.

## Current implementation status

As of now the current custom node retrieves all available devices from pilight and uses a config node which holds the hostname/ip of the pilight host and the port.
For now a hard coded pilight switch of type pollin is used for all nodes but the pilight device name and it's device artefacts is planned to be used instead.

## Sample flow which just turns a switch on and off

In following flow LivingRoom is the pilight switch node and pilightSend is a HTTP-Request node. The pilightSend node is supposed to vanish.

![Alt text](pics/pilight_customnode_flow.png?raw=true "Title")
