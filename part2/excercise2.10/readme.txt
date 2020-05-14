Changes needed:

The backend and frontend URLs in the Dockerfiles had to be changed to match the nginx configuration:

Frontend: API_URL=http://localhost/api/
Backend: FRONT_URL=http://localhost

