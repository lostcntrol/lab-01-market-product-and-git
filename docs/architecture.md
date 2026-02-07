## Product Choice
Name: Wildberries
Website: https://www.wildberries.ru
Description: Wildberries is a Russian marketplace. It was founded in 2004.

## Main components
![Wildberries Component Diagram](/docs/diagrams/out/wildberries/architecture-component/Component%20Diagram.svg)
![Link to PlantUML](/docs/diagrams/src/wildberries/architecture-component.puml)
[Customer Mobile App] - app for users to buy products
[Catalog & Search Service] - service with catalog of products
[PVZ Management Service] - service for managment of PVZ
[Fintech & Payment Service] - service for financial operations
[Review & Rating service] - service for users' reviews

## Data flow
![Wildberries Sequence Diagram](/docs/diagrams/out/wildberries/architecture-sequence/Sequence%20Diagram.svg)
![Link to PlantUML](/docs/diagrams/src/wildberries/architecture-sequence.puml)
[Preparation ] - customer search products and add them to the cart

## Deployment
![Wildberries Deployment Diagram](/docs/diagrams/out/wildberries/architecture-deployment/Deployment%20Diagram.svg)
![Link to PlantUML](docs/diagrams/src/wildberries/architecture-deployment.puml)
Main components are deployed in user computer and compute cluster

## Assumptions
I assume the Inventory Management system uses real-time predictive analytics to anticipate seasonal demand and automate stock replenishment across regional warehouses. I assume the Customer Personalization engine leverages machine learning algorithms to analyze browsing history and provide hyper-localized product recommendations based on regional trends.

## Open questions
How does the High-Load Architecture maintain system stability during peak sales events, such as 'Black Friday,' when concurrent user requests can surge by over 1000% in a single hour? To what extent does the Automated Sorting System utilize computer vision to identify and categorize mislabeled items before they enter the final 'last-mile' delivery stage