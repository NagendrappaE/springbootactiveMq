#spring boot3 with inmemeory active MQ demo with one queue 
#The below curl posts the status from CBS  to Broker 
curl -i http://localhost:8080/payment-status/post-to-queue/succes/123


other side the consumers will listen .
