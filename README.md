customer-segmentation-engine
Real-time customer segmentation and personalization engine using Java, Kafka, and ML scoring
Overview
customer-segmentation-engine is a Java backend service that ingests behavioral signals, segments customers in real time, and delivers personalized offer recommendations — modeled after enterprise decisioning systems built at Verizon serving millions of customers.
Tech Stack

Java 17 + Spring Boot 3
Apache Kafka — real-time event ingestion
Redis — caching and session data
PostgreSQL — customer profiles and history
REST APIs — offer delivery layer
Docker + Docker Compose
GitHub Actions CI/CD

Architecture
Behavioral Signal → Kafka → Segmentation Engine → ML Scoring → Offer Assignment → REST API
Endpoints
MethodEndpointDescriptionPOST/api/signalsIngest behavioral signalGET/api/segment/{customerId}Get customer segmentPOST/api/offers/recommendGet personalized offerGET/api/offers/history/{customerId}Get offer history
Getting Started
git clone https://github.com/saisrikanth-narina/customer-segmentation-engine
cd customer-segmentation-engine
docker-compose up
./mvnw spring-boot:run
Status
🚧 Active development — building week by week
