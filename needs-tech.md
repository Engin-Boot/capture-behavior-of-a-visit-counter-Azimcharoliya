# Visit-counter technical needs

Scenario: Recover across restarts of the server
that runs the visit-counter

  Given the server maintains the visitor count\
  When the server restarts\
  Then recover the count from server data and
  start counting visitors from that server count.

Scenario: Reconcile counts if the sensor is offline for a while

  Given the server maintains the visitor count\
  When the server is offline\
  Then we manually count the visitor till server is offline
  and update the count in server when server becomes available.
