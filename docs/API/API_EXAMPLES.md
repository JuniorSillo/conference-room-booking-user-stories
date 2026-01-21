# API Usage Examples for Conference Room Booking System

This document provides realistic examples of how to use the API. Examples use `curl` for simplicity, but you can adapt to any HTTP client (e.g., Postman, JavaScript fetch). Assume the base URL is `https://api.conferencerooms.example.com` 

All auth-required requests need a Bearer JWT token. Obtain one via a login endpoint.

## Authentication
Most endpoints require authentication. Example header:

`Authorization:` ~Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJzdWIiOiJ1c2VyLTc4OSIsImlhdCI6MTUxNjIzOTAyMn0.abcdef123456~


## Room Management
### List All Rooms
Retrieve all rooms.

`curl -X GET "https://api.conferencerooms.example.com/rooms" 
-H "Authorization: Bearer <token>"`

Expected response (200 OK):
`json
[
  {
    "id": "room-123",
    "name": "Boardroom A",
    "capacity": 10,
    "location": "Floor 5, Building HQ",
    "amenities": ["projector", "whiteboard"]
  }
]
`

## Create a New Room
### Add a room

``curl -X POST "https://api.conferencerooms.example.com/rooms" \
     -H "Content-Type: application/json" \
     -H "Authorization: Bearer <your-token>" \
     -d '{
           "name": "Meeting Room B",
           "capacity": 8,
           "location": "Floor 3, Building HQ",
           "amenities": ["video conferencing"]
         }'``
         
Expected response (201 Created): Similar to the room object above.

## Get a Specific Room
### Fetch details by ID.

`curl -X GET "https://api.conferencerooms.example.com/rooms/room-123" \
     -H "Authorization: Bearer <token>"`



## Bookings
### Create a Booking
#### Book a room (checks availability automatically).
`curl -X POST "https://api.conferencerooms.example.com/bookings" \
     -H "Content-Type: application/json" \
     -H "Authorization: Bearer <your-token>" \
     -d '{
           "roomId": "room-123",
           "userId": "user-789",
           "startTime": "2026-01-22T09:00:00Z",
           "endTime": "2026-01-22T10:00:00Z",
           "purpose": "Team meeting"
         }'`

         
## Expected response (201 Created): The booking object.
### List All Bookings
``curl -X GET "https://api.conferencerooms.example.com/bookings" \
     -H "Authorization: Bearer <token>"``

### Get a Specific Booking
``curl -X GET "https://api.conferencerooms.example.com/bookings/booking-456" \
     -H "Authorization: Bearer <token>"``
     
## Availability
### Check Room Availability for a Time Range
#### Public endpoint (no auth).
``curl -X GET "https://api.conferencerooms.example.com/availability?roomId=room-123&startTime=2026-01-22T09:00:00Z&endTime=2026-01-22T10:00:00Z"``

#### Expected response (200 OK):
``{
  "available": true,
  "conflictingBookings": []
}``

## Get Full Availability for a Room on a Date
``curl -X GET "https://api.conferencerooms.example.com/availability/room/room-123?date=2026-01-22" \
     -H "Authorization: Bearer <token>"``

#### Expected response: Array of available slots.
#### For error handling, e.g., if a booking conflicts, expect a 400 with an Error object.
