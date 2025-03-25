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
  "email": "exampleUser", ///string
  "password": "examplePassword" ///string
}
```

**Data Response Example:**

```json
{
  "status": "success/failed"
  "reason": "explanation"
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
  "email": <string>,
  "password": <string>,
  "first name": <string>,
  "last name": <string>,
  "age": <int>
}
```

**Data Response Example:**

```json
{
  "status": "success/failed"
  "reason": "explanation"
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
