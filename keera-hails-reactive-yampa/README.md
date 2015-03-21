This library contains functions to define RVs connected to Yampa signal
functions. The main function is yampaReactiveDual, which returns two RVs (a
readable end, or source, and a writable end, or sink).  You can write values
to the writable end, and changes will be processed by the SF and made
available in the readable end.

Yampa is a Functional Reactive Programming DSL.

Note: This library makes use of threads. You should compile your
executables using the threaded RTS (-threaded).

See also:
- http://github.com/keera-studios/keera-hails
- http://github.com/ivanperez-keera/Yampa
- http://github.com/keera-studios/hails-reactivevalues

# TODO

* Different update policies are possible. For instance, one could update only
  on demand, or update using a push policy. The yampa system could be running
  continuously, producing new outputs every time, and modifying the input only
  when it really changes.
