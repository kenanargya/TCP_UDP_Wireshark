# TCP_UDP_Wireshark

| Nama | NRP |
| ------- | ------- |
| Ken Anargya Alkausar | 5025211168  |

## TCP Problems

### 1. 
What is the IP address and TCP port number used by the client computer (source) that is transferring the alice.txt file to gaia.cs.umass.edu?
### 2. 
What is the IP address of gaia.cs.umass.edu? On what port number is it sending and receiving TCP segments for this connection?
### 3. 
What is the sequence number of the TCP SYN segment that is used to initiate the TCP connection between the client computer and gaia.cs.umass.edu? What is it in this TCP segment that identifies the segment as a SYN segment? Will the TCP receiver in this session be able to use Selective Acknowledgments (allowing TCP to function a bit more like a “selective repeat” receiver, see section 3.4.5 in the text)?
### 4. 
What is the sequence number of the SYNACK segment sent by gaia.cs.umass.edu to the client computer in reply to the SYN? What is it in the segment that identifies the segment as a SYNACK segment? What is the value of the Acknowledgement field in the SYNACK segment? How did gaia.cs.umass.edu determine that value?
### 5. 
What is the sequence number of the TCP segment containing the header of the HTTP POST command? How many bytes of data are contained in the payload (data) field of this TCP segment? Did all of the data in the transferred file alice.txt fit into this single segment?
### 6. 
Consider the TCP segment containing the HTTP “POST” as the first segment in the data transfer part of the TCP connection. 
* At what time was the first segment (the one containing the HTTP POST) in 
the data-transfer part of the TCP connection sent? 
* At what time was the ACK for this first data-containing segment received? 
* What is the RTT for this first data-containing segment? 
* What is the RTT value the second data-carrying TCP segment and its ACK?
* What is the EstimatedRTT value (see Section 3.5.3, in the text) after the ACK for the second data-carrying segment is received? Assume that in making this calculation after the received of the ACK for the second segment, that the initial value of EstimatedRTT is equal to the measured RTT for the first segment, and then is computed using the EstimatedRTT equation on page 242, and a value of  = 0.125.
### 7. 
What is the length (header plus payload) of each of the first four data-carrying TCP segments?
### 8. 
What is the minimum amount of available buffer space advertised to the client by gaia.cs.umass.edu among these first four data-carrying TCP segments7? Does the lack of receiver buffer space ever throttle the sender for these first four datacarrying segments?
### 9. 
Are there any retransmitted segments in the trace file? What did you check for (in the trace) in order to answer this question?
### 10. 
How much data does the receiver typically acknowledge in an ACK among the first ten data-carrying segments sent from the client to gaia.cs.umass.edu? Can you identify cases where the receiver is ACKing every other received segment (see Table 3.2 in the text) among these first ten data-carrying segments?
### 11. 
What is the throughput (bytes transferred per unit time) for the TCP connection? Explain how you calculated this value.
### 12. 
Use the Time-Sequence-Graph(Stevens) plotting tool to view the sequence number versus time plot of segments being sent from the client to the gaia.cs.umass.edu server.
### 13. 
These “fleets” of segments appear to have some periodicity. What can you say about the period?

## UDP Problems

### 1. 
Select the first UDP segment in your trace. What is the packet number4 of this segment in the trace file?
### 2. 
By consulting the displayed information in Wireshark’s packet content field for this packet (or by consulting the textbook), what is the length (in bytes) of each of the UDP header fields?
### 3. 
The value in the Length field is the length of what? (You can consult the text for this answer). Verify your claim with your captured UDP packet.
### 4. 
What is the maximum number of bytes that can be included in a UDP payload?
### 5. 
What is the largest possible source port number?
### 6. 
What is the protocol number for UDP?
### 7. 
Examine the pair of UDP packets in which your host sends the first UDP packet and the second UDP packet is a reply to this first UDP packet.
 
