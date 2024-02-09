# Django Blog API

## Overview
This Django Blog API offers a powerful and versatile backend solution tailored for blogging platforms. It stands out with its extensive range of endpoints, along with advanced authentication and authorization features. The API employs PostgreSQL as its database system, ensuring robust and efficient data management. Additionally, it utilizes Gunicorn as the WSGI HTTP Server for handling requests, enhancing its performance and scalability. Rigorously unit-tested, this API guarantees reliability and smooth operation. It's conveniently deployed on Heroku, providing straightforward access for testing and real-world application.


## Features
- **Endpoints:** A variety of routes for blog operations, including standard Django admin and user authentication routes.
- **Unit Testing:** Comprehensive tests for model validation, ensuring the integrity of blog posts.
- **Deployment:** Deployed on Heroku, showcasing the project's readiness for production environments.
- **Swagger UI and Redoc:** Integrated Swagger UI and Redoc for easy API documentation and exploration.
- **Authorization and Authentication:** Implemented robust security measures for user authentication and authorization.

## API Routes
- Admin: `"admin/"`
- Blog Posts: `"api/v1/"`
- Authentication: `"api-auth/"`
- REST Auth: `"api/v1/dj-rest-auth/"`
- Registration: `"api/v1/dj-rest-auth/registration/"`
- Schema: `"api/schema/"`
- Redoc: `"api/schema/redoc/"`
- Swagger UI: `"api/schema/swagger-ui/"`

## Environment Setup
Before running the project, you need to set up environment variables. Create a `.env` file in the project root with the following contents:

```plaintext
DEBUG=False
SECRET_KEY=<your_secret_key>
DATABASE_URL=sqlite:///db.sqlite3
```

These variables are crucial for configuring the Django settings properly.

## Running the Project
To run this project on your local machine, follow these steps:

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/Dandiggas/blogapi
   cd blogapi
   ```

2. **Set up a Virtual Environment:**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows use `venv\Scriptsctivate`
   ```

3. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

4. **Migrate the Database:**
   ```bash
   python manage.py migrate
   ```

5. **Run the Server:**
   ```bash
   python manage.py runserver
   ```

## Testing
To run the unit tests:

```bash
python manage.py test
```

The tests cover the following aspects:
- User model creation
- Post creation and field validation

## Deployment
The API is deployed on Heroku. You can access and test it at [Heroku Deployment](https://diggas-blog-api-8696c6144886.herokuapp.com/api/v1/dj-rest-auth/registration/). Note that registration is required to access the API.

## Documentation and Exploration
- **Swagger UI:** Explore the API using Swagger UI at `https://diggas-blog-api-8696c6144886.herokuapp.com/api/schema/swagger-ui/`
- **Redoc:** For a more detailed documentation, visit Redoc at `https://diggas-blog-api-8696c6144886.herokuapp.com/api/schema/redoc/`

## Security
This API implements robust security practices including user authentication and authorization to ensure data protection and privacy.

## Contributing
Contributions to the project are welcome. Please follow the standard fork, branch, and pull request workflow.


## Contact
For any inquiries or contributions, please contact Daniel Adekugbe at Danieladekugbe@gmail.com

---

This project is part of my backend portfolio, showcasing my skills in building reliable, secure, and well-documented APIs using Django.
