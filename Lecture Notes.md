#Notes


##Lecture Notes 1
- Cloud computing explains server architecture

###Types
- Client Server
	- master-slave relationship
- P2P
	- No master or slave, everyone can be client and server at same time

###Layered Architecture
- The more layers you add, less efficient

###3 different sql
- key-value NOSQL
- Document NOSQL
- Column-family NOSQL
- Graph NOSQL
- Hyper-Graph NOSQL Neo4j
	- Graph = (Node, Edge) where Edge = (Node1, Node2)


##Lecture Notes 2

###Programming Asignment 1

####What is Linda?
- Linda is a distributed model
- Logical, global tuple set
- Pretty old concept, 1980's

####2 Components
- server
	- should be run first, run forever
	
~~~~c++
	while (1) {
		socket();
		bind()
		listen()
		while(1) {
			accept()
			receive()
			send()
		}
	}	
~~~~

- client

~~~~c++
	socket()
	connect()
	send()
	receive()
	close()
~~~~


- port numbers
	- 0 - 65535 total
	- 0 - 1023 reserved
	- 1024 - 65535
	- Find a port which no one uses and use it
- Which tuples on which host?
	- Hash it using MD57 algorithm
	- ("abc", 3) -> "abc3"
	- (3.5, "def", 3, "xyz") -> "3.5def3xyz"
- IP Address
	- 129.210.16.XX


##Lecture Notes 4

- $MTTF, MTTR$
- $Utilization = \frac{MTTF}{MTTF+MTTR}$

###Architecture Design Challenges

##Lecture Notes 6

###Examples of Commercial Cloud Services
- Microsoft Azure
- Use APIs to get and put data, do not need to worry about backing up
- $K = 10^3, M = 10^6, G = 10^9, T = 10^12, P = qo^15, E = 10^18$


##Lecture Notes 7
- Harmony problem
	- Detect and disable
- Don't use java for real time (becaue you have to onvert to intermediate language)
- Sqquential program t
- n machine $\frac{T}{n}$, $\alpha, 1-\alpha$
- $\alpha T + \frac{T(1-\alpha)}{n}$
