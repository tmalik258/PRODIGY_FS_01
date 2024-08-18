# PRODIGY_FS_01 - Secure Authentication Project

This project is a secure authentication system built using Django REST Framework and Django REST SimpleJWT for the backend, with React as the frontend. The frontend communicates with the backend via Axios, and a custom hook `useUserActions` is used to manage user-related actions.

## Features

- **Secure Authentication**: JWT-based authentication using Django REST SimpleJWT.
- **User Registration & Login**: Users can register and log in securely.
- **Token Management**: Refresh and access tokens are managed for secure API interactions.
- **React Frontend**: A responsive frontend built with React.
- **Axios for API Requests**: Axios is used to handle all API requests.
- **Custom Hook `useUserActions`**: This custom hook manages user actions like login, logout, and registration.
- **Automated Tests**: `tests.py` written for backend unit testing.

## Prerequisites

- Python 3.x
- Django 4.x
- Node.js 14.x or later
- npm

## Backend Setup

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/tmalik258/prodigy_fs_01.git
   cd prodigy_fs_01
   ```

2. **Create a Virtual Environment:**

   ```bash
   python -m venv env
   source env/bin/activate  # On Windows use `env\Scripts\activate`
   ```

3. **Install Dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

4. **Run Migrations:**

   ```bash
   python manage.py migrate
   ```

5. **Create a Superuser:**

   ```bash
   python manage.py createsuperuser
   ```

6. **Run the Development Server:**

   ```bash
   python manage.py runserver
   ```

## Running Tests

- **Run All Tests:**

  ```bash
  python manage.py test
  ```

This will execute the tests defined in `tests.py` to ensure the backend functions as expected.

## Frontend Setup

1. **Navigate to the Frontend Directory:**

   ```bash
   cd ../frontend
   ```

2. **Install Dependencies:**

   ```bash
   npm install
   ```

3. **Start the Development Server:**

   ```bash
   npm start
   ```

## Usage

- Access the backend API at `http://localhost:8000/api/`.
- Access the frontend at `http://localhost:5173/`.

### Custom Hook: `useUserActions`

This custom hook is responsible for handling user-related actions such as login, logout, and registration. It interacts with the backend API using Axios and manages JWT tokens.

## Folder Structure

```plaintext
prodigy_fs_01/
│
├── manage.py
├── core/
├── users/
│   ├── tests.py
│   ├── ...
├── auth/
│   ├── tests.py
│   ├── ...
│
├── frontend/
│   ├── src/
│   ├── public/
│   ├── ...
│
└── README.md
```

## License

This project is licensed under the MIT License.
