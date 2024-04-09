# Ninjas API Documentation

This is a RESTful API built with NestJS for managing Ninjas. The API allows you to create, read, update, and delete Ninjas.

## Endpoints

### GET /ninjas

This endpoint retrieves all ninjas. You can filter the ninjas by their weapon type by passing the 'weapon' query parameter. The 'weapon' parameter can be either 'stars' or 'nunchucks'.

### GET /ninjas/:id

This endpoint retrieves a single ninja by their ID.

### POST /ninjas

This endpoint creates a new ninja. The request body should be a JSON object that follows the `CreateNinjaDto` schema.

### PUT /ninjas/:id

This endpoint updates a ninja by their ID. The request body should be a JSON object that follows the `UpdateNinjaDto` schema.

### DELETE /ninjas/:id

This endpoint deletes a ninja by their ID.

## DTOs

### CreateNinjaDto

This is the schema for creating a new ninja.

### UpdateNinjaDto

This is the schema for updating an existing ninja.

## Services

### NinjasService

This service contains the business logic for managing ninjas. It is responsible for getting all ninjas, getting a single ninja by their ID, creating a new ninja, updating a ninja, and deleting a ninja.

## Modules

### NinjasModule

This module imports and provides the `NinjasController` and `NinjasService`.

## Controllers

### NinjasController

This controller handles HTTP requests and responses for the ninjas API. It uses the `NinjasService` to perform operations.

## Running the API

To run the API, use the following command:

```bash
npm run start
```

## Testing the API

To test the API, use the following command:

```bash
npm run test
```

## Contributing

If you want to contribute to this project, please make sure to follow the coding standards and write tests for your features or bug fixes.

