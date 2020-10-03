# kafka-bigdata-group1
## Prasanna Kumar
**Github Profile:** [https://github.com/prasu93](https://github.com/prasu93)
## Omkar Abhiteja Badda
**Github Profile:** [https://github.com/abhiteja29](https://github.com/abhiteja29)
## Yugandhar Mamidi
**Github Profile:** [https://github.com/yugandharmamidi](https://github.com/yugandharmamidi)
## Gangadhar Yerramsetti
**Github Profile:** [https://github.com/gangadhary574](https://github.com/gangadhary574)

## Team Lead Commands (Prasanna)
Step1 : Zookeeper service -> Run the below command from the kafka folder:

`.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties`

Step2 : Kafka service -> Run the below command from the kafka folder:

`.\bin\windows\kafka-server-start.bat .\config\server.properties`

Step3 : The structure and application code is available at

`src\main\java\edu\nwmissouri\kafkabigdatagroupapp\`

Step4 : Fat jar file creation-> Run the below command from the root folder of the java project

`mvn clean compile assembly:single`

Step5 : Start the Consumer: Run the below command from the root folder of the project. I have taken topic as test and group as group

`java -cp .\target\kafka-bigdata-group-app-1.0-SNAPSHOT-jar-with-dependencies.jar com.edu.nwmissouri.kafkabigdatagroupapp.simple.Consumer test group`

Step6 : Start the Producer:

`java -cp .\target\kafka-bigdata-group-app-1.0-SNAPSHOT-jar-with-dependencies.jar com.edu.nwmissouri.kafkabigdatagroupapp.simple.MamidiProducer test`

Now, any valid Producer can send messages to the the Consumer.

## Mamidi(Producer and Consumer Commands)
Producer command:
`java -cp .\target\kafka-bigdata-group-app-1.0-SNAPSHOT-jar-with-dependencies.jar edu.nwmissouri.kafkabigdatagroupapp.simple.MamidiProducer apple-products`

Consumer command:
`java -cp .\target\kafka-bigdata-group-app-1.0-SNAPSHOT-jar-with-dependencies.jar edu.nwmissouri.kafkabigdatagroupapp.simple.Consumer apple-products edu.nwmissouri.kafkabigdatagroupapp.simple`


## Yerramsetti(Producer)

Producer command:
`java -cp .\target\kafka-bigdata-group-app-1.0-SNAPSHOT-jar-with-dependencies.jar edu.nwmissouri.kafkabigdatagroupapp.simple.GangadharProducer college-admissions`

Consumer command:
`java -cp .\target\kafka-bigdata-group-app-1.0-SNAPSHOT-jar-with-dependencies.jar edu.nwmissouri.kafkabigdatagroupapp.simple.Consumer college-admissions group`

## Badda(Producer)

Consumer command:
`java -cp .\target\kafka-bigdata-group-app-1.0-SNAPSHOT-jar-with-dependencies.jar edu.nwmissouri.kafkabigdatagroupapp.simple.Consumer ios14-features group`

Producer command:
`java -cp .\target\kafka-bigdata-group-app-1.0-SNAPSHOT-jar-with-dependencies.jar edu.nwmissouri.kafkabigdatagroupapp.simple.BaddaProducer ios14-features`

--

