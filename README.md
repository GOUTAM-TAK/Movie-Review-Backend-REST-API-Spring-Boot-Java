Use Case: Movie review system
Description:
Develop RESTful services for a Movie revies  where a user add a review to the movie

Create User n Movie entities suitably

Review attributes  : like review ID(PK auto generated), review contents,rating,user id (FK) , movie id (FK)


Endpoints:
1.	Get all reviews
This should return a JSON containing : review id , review contents , rating
•	GET /reviews/{reviewId}
•	Request: Retrieve details of a specific review by providing its unique identifier.
•	Response: JSON representation of the review.
2.	Add a review
•	Endpoint: POST /reviews
•	Request: JSON payload(DTO)  containing review details (review contents,contents,user id, movie id)
•	Response: Confirmation of the created review .
3.	Update review:
•	Endpoint: PUT /reviews/{reviewId}
•	Request: Update an existing recipe by providing its unique identifier and the updated information.
•	Response: Confirmation of the updated recipe.
4.	Delete Recipe:
•	Endpoint: DELETE /reviews/{reviewId}
•	Request: Delete a review by providing its unique identifier.
•	Response: Confirmation of the deleted review.

Notes:
•	Response codes should be as per REST guidelines.
•	Error handling in case of failures.
