# Map-Reduce-job--RowCount
Map-Reduce job computes the number of rows in the text file

# Unix commands
## Running Map-Reduce using jar file

hadoop fs -put data.txt /user/cloudera/

hadoop fs -ls /user/cloudera

hadoop jar cards_mr.jar lab.cards.RowCount /user/cloudera/data.txt /user/cloudera/output

hadoop fs -ls /user/cloudera/output

hadoop fs -cat /user/cloudera/output/part-r-00000
