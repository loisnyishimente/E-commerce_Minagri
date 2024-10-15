# E-Commerce Order Processing System

## Class Design

### Object-Oriented Principles Applied

- **Abstraction**: The `OrderItem` abstract class provides a template for all types of items. Specific item classes (e.g., `PhysicalProduct`, `DigitalProduct`, and `GiftCard`) extend this class and implement their specific behaviors.
- **Inheritance**: Each product type inherits common attributes and methods from the `OrderItem` class, allowing for code reuse.
- **Polymorphism**: Each concrete class implements its methods, allowing the system to treat all order items uniformly while still supporting individual behavior.

### API Endpoints

- **Create Order**
    - **HTTP Method**: `POST`
    - **URL Pattern**: `/orders`
    - **Request Body**: [See example above]
    - **Response**: [See example above]

- **Get Order by ID**
    - **HTTP Method**: `GET`
    - **URL Pattern**: `/orders/{id}`
    - **Response**: [See example above]

### Scalability and Extensibility

This design allows for easy addition of new product types by simply creating new classes that extend `OrderItem` and implement the relevant interfaces. For example, if we wanted to add a new `SubscriptionProduct`, we would create a new class that defines its specific behaviors while still adhering to the common structure defined by `OrderItem`.

## Testing Instructions

1. Clone the repository.
2. Run the main application.
3. Use tools like Postman to test the API endpoints.
4. Create orders using the specified JSON format and observe the output.

## Git Repository


