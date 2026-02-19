# Scarlett Automation Starter v4 Documentation

## Fanvue API

### Overview
The Fanvue API allows developers to interact with Fanvue's services programmatically. This documentation provides an overview of endpoints, authentication, and usage examples.

### Authentication
To access the Fanvue API, you need to obtain an API key. This key must be included in the header of each request.

**Header Format:**
```
Authorization: Bearer YOUR_API_KEY
```

### Endpoints

#### 1. Get User Information
- **Endpoint:** `/api/user`
- **Method:** `GET`

**Description:** Retrieves information about the authenticated user.

**Example Request:**
```bash
curl -H "Authorization: Bearer YOUR_API_KEY" https://api.fanvue.com/api/user
```

#### 2. Get Posts
- **Endpoint:** `/api/posts`
- **Method:** `GET`

**Description:** Fetches posts made by the user.

**Example Request:**
```bash
curl -H "Authorization: Bearer YOUR_API_KEY" https://api.fanvue.com/api/posts
```

#### 3. Create Post
- **Endpoint:** `/api/posts`
- **Method:** `POST`

**Description:** Creates a new post.

**Example Request:**
```bash
curl -X POST -H "Authorization: Bearer YOUR_API_KEY" -H "Content-Type: application/json" -d '{"content":"Your post content here"}' https://api.fanvue.com/api/posts
```

### Error Handling
The API returns standard HTTP status codes. In case of an error, a JSON response will be provided with an error message.

### Rate Limiting
Be aware that the Fanvue API has rate limits. Exceeding these limits will result in a `429 Too Many Requests` response.

### Conclusion
For further details, refer to the official Fanvue API documentation.

---

**Credits:** This document was generated on 2026-02-19.