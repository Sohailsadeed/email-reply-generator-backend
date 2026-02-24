# 📧 Email Reply Generator – Spring Boot Backend

Spring Boot backend service that generates AI-powered email replies using Gemini API. Built with clean layered architecture and integrated with a Chrome Extension frontend.

---

## 🚀 Tech Stack

- Java 17+
- Spring Boot
- Spring WebFlux (WebClient)
- Maven
- Gemini API

---

## 🔌 API

POST `/api/email/generate`

### Request

```json
{
  "emailContent": "Original email text",
  "tone": "professional"
}
```

### Response
Plain text AI-generated reply.

---

## 🔐 Environment Variables

Set the following before running:

```
GEMINI_API_URL
GEMINI_API_KEY
```

Configure in `application.properties`:

```
gemini.api.url=${GEMINI_API_URL}
gemini.api.key=${GEMINI_API_KEY}
```

Never commit API keys.

---

## ▶️ Run

```bash
mvn spring-boot:run
```

Runs on:

```
http://localhost:8080
```

---

## 🔮 Future Enhancements

- Database integration (Spring Data JPA)
- AOP-based logging
- Authentication & rate limiting
