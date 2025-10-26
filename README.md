##this will be acting as activemq broker server as running on tcp://localhost:61616
#spring boot3 with inmemeory active MQ demo with one queue 
#The below curl posts the status from CBS  to Broker 
curl -i http://localhost:8080/payment-status/post-to-queue/succes/123


other side the consumers will listen .


#active MQ quque consumer service is there ,it will use the  activeMq server to conume the services ,
ex: i will post the account details into active Mq server using queue Name ACCOUNT_STATUS_QUEUE
curl -i http://localhost:8080/account-status/post-to-queue/succes/123


The consumer application will consume @ listner using that data

