
# Pass-in

Pass-in handles events and attendees smoothly!




## Tech Stack

- Java with Maven
- Spring Boot
- API Rest
- HSQL


## API Reference

### Post event

```http
  POST /events
```

#### Event post usage/example
```
{
	"title": "Event Test 2.0",
	"details": "A cool description",
	"maximumAttendees": 10
}
```

### Get event

```http
  GET /events/{eventId}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `eventId` | `string` | Show event |

### Post attendee

```http
  POST events/{eventId}/attendees
```

#### Attendee post usage/example
```
{
	"name": "Ahsoka Tano",
	"email": "ahsokatano@outlook.com"
	
}
```

### Get attendees

```http
  GET /events/attendees/{eventId}
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `eventId` | `string` | Show attendees |

### Get badge

```http
  GET attendees/{attendeeId}/badge
```

| Parameter | Type     | Description                |
| :-------- | :------- | :------------------------- |
| `attendeeId` | `string` | Show badge |

### Post attendee

```http
  POST attendees/{attendeeId}/check-in
```

