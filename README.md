# viewDataFromDataBase

## Examples

### Transcript

**Endpoint:**

```
GET /videos/2tM1LFFxeKg/questions
```

**Data Response Example:**

[Transcript JSON](https://raw.githubusercontent.com/The-JAR-Team/viewDataFromDataBase/refs/heads/main/transcripts/2tM1LFFxeKg_transcript.JSON)

### All Videos

**Endpoint:**

```
GET /videos
```

**Data Response Example:**

[Video Metadata JSON](https://raw.githubusercontent.com/The-JAR-Team/viewDataFromDataBase/refs/heads/main/fetch/video_metadata.json)

### User Login

**Endpoint:**

```
POST /login
```

**Request Body Example:**

```json
{
  "username": "exampleUser",
  "password": "examplePassword"
}
```

**Data Response Example:**

```json
{
  "token": "exampleToken", /// or authToken ...??
  "userId": "exampleUserId"
}
```

### User Registration

**Endpoint:**

```
POST /register
```

**Request Body Example:**

```json
{
  "username": "newUser",
  "password": "newPassword",
  "email": "newUser@example.com"
}
```

**Data Response Example:**

```json
{
  "userId": "newUserId", /// optinal???
  
  "status": "success" // or
}
```

### Add Video

**Endpoint:**

```
POST /videos
```

**Request Body Example:**

```json
{
  "title": "New Video Title",
  "group": "Description of the new video",
  "url": "http://example.com/new-video-url",
  "upload by" : "team teen"
}
```

**Data Response Example:**

```json
{
  "videoId": "newVideoId",
  "status": "success"
}
