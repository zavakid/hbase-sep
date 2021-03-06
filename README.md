HBase Side-Effect Processor
===========================

The HBase Side-Effect Processor is a framework for handling HBase row mutation events (i.e. Put and Delete) asynchronously. The framework makes use of the built-in HBase replication functionality, and allows users to register EventListeners which will be notified when a row mutation occurs in HBase.

This approach is significantly different from the use of Coprocessors due to it being asynchronous -- the distribution of events and execution of event handlers has no direct impact on write throughput in HBase.

To get started with the HBase-SEP, try playing with the included demo sub-project.

HBase SEP has been created as part of the hbase-indexer project - http://github.com/NGDATA/hbase-indexer.
