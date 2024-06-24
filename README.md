# loginauth
Django project with DRF and JWT (email-password) authentication system by customizing UserModel and Serializer

Step 1: 
-Make sure the Django server is running.
"python manage.py runserver"

Step 2:
We will use Postman to test the API endpoint.
- Open Postman.
- Create a new POST request.
- Set the URL to http://127.0.0.1:8000/api/register/
- Set request body to 'JSON' and include following:
     {
      "email": "test@123.com",
      "password": "test123",
      "first_name": "Test",
      "last_name": "User"
      }
- Send the request.

- Similarly for login change the URL to http://127.0.0.1:8000/api/login/ and include following:
    {
    "email": "testuser@example.com",
    "password": "testpassword123"
    }
- The login will be successful and should receive response with JWT token.


  
