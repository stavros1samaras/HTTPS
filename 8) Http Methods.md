# HTTP Methods

## What they are
HTTP methods define **what action the client wants the server to perform** on a resource.

## Main HTTP Methods

### GET
- Used to **request data** from a resource.
- Does **not** modify anything.
- Common for loading pages.

### POST
- Used to **send data** to the server.
- Usually for **creating** a new resource.
- Contains a request body.

### PUT
- **Replaces** an existing resource entirely.
- Full update.

### DELETE
- Deletes the specified resource.

### HEAD
- Same as GET **but without the response body**.
- Used to check metadata (e.g., size, last-modified).

### PATCH
- **Partially updates** a resource.
- Contains a request body.

### OPTIONS
- Returns the communication options and supported methods for a resource.
- Used heavily in **CORS**.


## Important Notes

### 1. HTTP methods appear **only in requests**, never in responses.
- Request example: `GET /users`
- Response example: `200 OK` (status code, not a method)

### 2. A request can contain **only one method**.
- You cannot have GET + POST in the same request.

### 3. POST, PUT, PATCH typically have bodies.
- GET and HEAD usually do not.

### 4. Loading a webpage creates **many HTTP requests**, not just one.
- HTML, CSS, JS, images, fonts, etc.

### 5. Some methods are often blocked
