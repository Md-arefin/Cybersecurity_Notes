# LAYERED TASKS

## THE OSI MODEL
Established in 1947, the International Standards Organization (ISO) is a multinational
body dedicated to worldwide agreement on international standards. An ISO standard
that covers all aspects of network communications is the Open Systems Interconnection
model. It was first introduced in the late 1970s. An open system is a set of protocols that
allows any two different systems to communicate regardless of their underlying architecture. The purpose of the OSI model is to show how to facilitate communication
between different systems without requiring changes to the logic of the underlying hardware and software. The OSI model is not a protocol; it is a model for understanding and
designing a network architecture that is flexible, robust, and interoperable.

ISO is the organization. OSI is the model.

The OSI model is a layered framework for the design of network systems that allows communication between all types of computer systems. It consists of seven separate but related layers, each of which defines a part of the process of moving information
across a network

### Layered Architecture
The OSI model is composed of seven ordered layers: 
- physical (layer 1), 
- data link (layer 2),
- network (layer 3), 
- transport (layer 4), 
- session (layer 5), 
- presentation (layer 6), and
- application (layer 7).


Layer 3, for example, uses the services provided by layer 2 and provides services for layer 4. Between machines, layer x on one machine communicates with layer x on another machine. 

This communication is governed by an agreed-upon series of rules and conventions called protocols. 

The processes on each machine that communicate at
a given layer are called peer-to-peer processes.

Communication between machines is therefore a peer-to-peer process using the protocols appropriate to a given layer.