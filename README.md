Jms Rollback No Transactions
============================

This application demonstrates the use of Rollback Exception Strategy on Jms and transactions. The use-case is to attempt redelivery
the configured amount of times and then upon exhaustion, forward the message to the dead letter queue as well as stopping processing
of subsequent messages on the queue. This can be done by stopping the flow. We stop the flow by accessing it by name on the app.registry

Version
=======
3.4

Contact
=======
nial.darbey@mulesoft.com