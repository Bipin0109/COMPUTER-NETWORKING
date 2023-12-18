# Computer-Networks
Various real life problem statements are provided. We need to solve those problems using networking logic in C language. Figuring out the problem through using the logics of Computer Networks
#Problem Statement : [ In real world scenario] There is a OTT platform , where three processes involve together to complete the system's functionality like publishing , subscribing and watching some content. In the system many publishers may exist . Many subscribers may also exist . For each subscriber option of selecting different publisher's content should be displayed. And after subscribing subscriber should only get the content of those publishers for which they have subscribed.

Problem Statement : [In terms of Networking] There exist multiple publisher process which are handled by the Dispatcher process using pthreads and multiple users which are also handled by the dispatcher at another socket file descriptor(sfd). Communicating between these processes using TCP Socket. Data from one Publisher should get to every Subscriber who has opted for that publisher;s content.

Sequence of system calls and IPCs used:

TCP connection between P and D.
TCP between S and D.
threads for handling multiple processes of P and S concurrently.
Raw socket for Broadcasting the same message to selected S process.
