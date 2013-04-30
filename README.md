Jms Rollback No Transactions
============================

This application demonstrates the use of Rollback Exception Strategy on Jms and transactions. The use-case is to attempt redelivery
the configured amount of times and then upon exhaustion, leave the message on the queue without committing the transaction. In order to leave the message
on the queue, one needs prevent transaction commit. This can be done by stopping the flow. When the subsequent commit is attempted, it will fail because the
flow is already stopped.

We stop the flow by accessing it by name on the app.registry

Version
=======
3.4

Contact
=======
nial.darbey@mulesoft.com