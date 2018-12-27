<!-- TITLE: Data Compression -->
<!-- SUBTITLE: A quick summary of Data Compression -->

# Data Compression
Data compression and compression formats can have a significant impact on performance. Three important places to consider data compression are in MapReduce and Spark jobs, data stored in HBase, and Impala queries. For the most part, the principles are similar for each.
You must balance the processing capacity required to compress and uncompress the data, the disk IO required to read and write the data, and the network bandwidth required to send the data across the network. The correct balance of these factors depends upon the characteristics of your cluster and your data, as well as your usage patterns.
Compression is not recommended if your data is already compressed (such as images in JPEG format). In fact, the resulting file can sometimes be larger than the original.