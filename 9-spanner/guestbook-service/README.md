# gcloud spanner instances create message-instance --config=regional-us-central1 --nodes=1 --description="Guestbook messages"
# gcloud spanner databases create guestbook_message --instance=message-instance
# gcloud spanner databases ddl update guestbook_message --instance=message-instance --ddl="$(<db/spanner.ddl)"

#./mvnw spring-boot:run -Dserver.port=8081 -Dspring.profiles.active=cloud
#curl http://localhost:8081/guestbookMessages
#curl -XPOST -H "content-type: application/json" -d '{"name": "John Doe", "message": "Hello Cloud Spanner"}'
#curl -XPOST -H "content-type: application/json" -d '{"id":"1234", name": "Mary Doe", "message": "Hello Cloud Spanner"}'
