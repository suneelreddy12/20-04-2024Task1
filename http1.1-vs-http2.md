# Evolution of HTTP: A Comparative Analysis of HTTP/1.1 and HTTP/2 #

HTTP - Hypertext Transfer Protocal

## Multiplexing

- In HTTP/1.1, each request was processed sequentially, meaning that if one request was slow or blocked, 
it could hold up subsequent requests, leading to latency issues
- One of the most notable features of HTTP/2 is multiplexing, which allows multiple requests and responses to be sent and received
 in parallel over a single TCP connection. Unlike HTTP/1.1, where each request had to wait for previous ones to complete, 
  multiplexing enables more efficient resource utilization and significantly reduces latency.

## Header Compression

- HTTP/2 employs header compression techniques to reduce overhead, which was a notable issue in HTTP/1.1 due to the verbose nature
of headers. By using Huffman encoding and other compression algorithms(HPACK, ...etc), HTTP/2 minimizes the size of headers, 
leading to faster transmission of data and reduced bandwidth consumption.

## Binary Protocal

- In HTTP/1.1, communication between clients and servers is done using a textual format, where messages are represented in plain text.
This means that data is encoded using characters from the ASCII or Unicode character sets, making it human-readable but
potentially verbose. In contrast, HTTP/2 adopts a binary framing layer, where messages are encoded in binary format, 
consisting of sequences of 0s and 1s. This binary format is machine-readable but not human-readable without special tools.