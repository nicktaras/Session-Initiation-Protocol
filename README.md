# SIP - Session Initiation Protocol

SIP - Learning

# HISTORY:

### Analogue
[TIP & Ring Telephony]

### Digital 
[Phone System - dedicated ethernet connections]

### VoIP
[Shared high speed network, using the same network for internet and phone]
(Cheaper, this is where SIP showed up to provide a solution to this).

### The POTS Line (Analogue)

- Analogue
- Plain old Tele service
- Two Wires
- Voltage sends ringing
- Closed Circuit Connects Phones (when both phones are picked up the circuit connects)

ONE of the most reliable ways of communication, even today. 

### T1/E1 PRI (Primary Interface)

- Digital
- T1 = 24 Channels
- E1 = 32 Channels
- Contains B Channels (calls) and one Channel D (Signalling - trying to make call, waiting)
- Limited redundancy capabilities

### SIP Trunking

- VOIP
- Unlimited Channels, contstrained by Bandwidth
- Delivery over IP Circuits (Internet, Dedicated, MPLS)
- Many redundancy capabilities (flexible, to re-direct keep online)

## SIP:

- It changes the playing field, because it was an Open Standard (modern telephony over IP)
- Cisco, tried to do the same thing (to make money out of the open standard)
- SIP, wasn't made for VOIP, it was made to manage the State of a System, but adopted for VoIP

### Versatile

- Calls
- Instant messaging
- Presence

### SIP Signalling

- Keep Alive (options)
- SIP Register, is an alternative to Keep Alive (A provider determines the rules)
- I need to make a call, "SIP INIVTE"
- I'm trying to make a call "SIP TRYING"
- I've found a destination and rining it ("RINING")
- End call ("BYE")

### SIP Messages

- Provisional Responses 100 messages

A. 100 'Trying' (Server knows I'm working on connecting)
B. 180 'Ringing'
C. 181 'Call being forwarded'
D. 183 'Session Progress' Information is being established

100 - doens't ring.
180 - means it's actually ringing

- 200 messages

A. Success 200
B. Accepted 202, but not done on the server side

- 300 messages, Redirect Responses

A. 300 Mulitple Choices (destination found, but many options)
B. 301 Moved permanently 
C. 302 Move Temporarily
D. 305 Use Proxy, info about how to re-connect with Proxy

- 400 messages, Redirect Responses

A. 400 bad request
B. 401 unauthorised (send another message with auth)
C. 403 forbidden
D. 404 not found
E. 405 Method not found
F. 408 Timeout, disconnect
G. 480 Temporairily unavailble
H. 488 Not going to handle this request

- 500 messages, Server Failure Responses
- 600 messages, Global Failure Responses (Rare occurances)

### SIP Media

RTP - Real Time Protocol (Stream of Traffic)
RTCP - Real time Control Protocol
SDP - Session Description Protocol
Media Path - Transmitted via RTP
Two Streams - One in each direction
Media Path communucation - during set up call
Media stream can change mid call
- SDP, change made during call
- Music on hold

### SDP - Session Description Protocol

- Info about media establishment, codec, what type of media, which port.

v=0 - is a session identifer 
o= is a username and 1 side of connection IP
s= is a session name
u= resource
e= email
c= Connection data (direction) IP
t= 
a= Type e.g. recieve only
m=
m=
a=
























