# Airbnb Clone - Backend Architecture

## Core Components
### 1. User Authentication & Management

![auth](./images/user-auth.png)

#### Endpoints:

- `POST /api/auth/register/` - User registration

- `POST /api/auth/login/` - JWT token generation

- `GET /api/users/` - Current user profile

- `PATCH /api/users/` - Update profile

### 2. Property Management

![](./images/property-management.png)

#### Endpoints:

- `POST /api/properties/` - Create listing

- `GET /api/properties/?filters` - Search listings

- `PUT /api/properties/{id}/` - Update listing

- `POST /api/properties/{id}/media/` - Upload images

### 3. Booking System

![](./images/bookings.png)

#### Endpoints:

- `POST /api/bookings/` - Create booking

- `GET /api/bookings/upcoming/` - Upcoming stays

- `PATCH /api/bookings/{id}/` - Modify booking

- `POST /api/bookings/{id}/cancel/` - Cancel booking

### 4. Payment Processing

![](./images/payments.png)

#### Endpoints:

- `POST /api/payments/intent/` - Create payment intent

- `POST /api/payments/confirm/` - Confirm payment

- `GET /api/payments/transactions/` - Payment history

### 5. Review System

![](./images/reviews.png)

#### Endpoints:

- `POST /api/reviews/` - Submit review

- `GET /api/properties/{id}/reviews/` - Property reviews

- `POST /api/reviews/{id}/respond/` - Host response


## Complete Design

![](./images/complete.png)