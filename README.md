# MicroNest

MicroNest is a robust application demonstrating the power of .NET Core with a comprehensive microservices architecture. This project leverages multiple microservices to handle various aspects of product and order management, ensuring high scalability, maintainability, and flexibility.

<div style="display: flex; flex-wrap: wrap; gap: 10px;">
 <img width="400" alt="1" src="https://github.com/karabasnejat/NetCoreAppWithMicroServices/assets/62561906/add364ce-a16a-4043-9fa8-50860f1730b1">
 <img width="400" alt="2" src="https://github.com/karabasnejat/NetCoreAppWithMicroServices/assets/62561906/93f4be8c-6af8-442f-89d2-95d4a387cda1">
 <img width="400" alt="3" src="https://github.com/karabasnejat/NetCoreAppWithMicroServices/assets/62561906/314945e9-39ba-4f63-ad7c-67ff3bb9a75f">
 <img width="400" alt="4" src="https://github.com/karabasnejat/NetCoreAppWithMicroServices/assets/62561906/2ccd2723-7887-4c6a-b06d-ac01ffc2fbbc">
 <img width="400" alt="5" src="https://github.com/karabasnejat/NetCoreAppWithMicroServices/assets/62561906/347344c6-3477-400d-8cb5-97c6ca6d2c9f">
 <img width="400" alt="6" src="https://github.com/karabasnejat/NetCoreAppWithMicroServices/assets/62561906/61e6a4c8-c523-4568-983b-e31021216d49">
  
</div>

## Features

- **Product Management**: Extensive CRUD operations for product data.
- **Order Management**: Real-time tracking and management of orders.
- **API Gateway**: Facilitates secure and efficient communication between services.
- **Responsive Design**: Utilizes Tailwind CSS for a modern and responsive UI.
- **Scalability**: Efficiently handles over 10,000 records in both product and order services.
- **Uptime Monitoring**: Includes an Uptime Robot to monitor service health and status.

## Technologies Used

- **ASP.NET Core 7.0**: Backend services and API development.
- **Entity Framework Core**: Efficient data management and ORM.
- **Ocelot API Gateway**: Secure routing between microservices.
- **Tailwind CSS**: Modern, responsive design framework.
- **Node.js**: Additional backend services and utilities.
- **N-Tier Architecture**: Separates concerns across different layers, improving maintainability.

## Microservices Architecture

MicroNest is composed of the following microservices:

- **ProductService**: Handles all operations related to product data.
- **OrderService**: Manages order processing, tracking, and data.
- **API Gateway**: Manages requests between the client and microservices, providing a single entry point.

Each service is independently deployable and scalable, allowing for efficient resource management and easier updates.

## Getting Started

### Prerequisites

- .NET Core SDK
- Node.js
- Docker (optional, for containerization)

### Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/enesscigdem/NetCoreAppWithMicroServices.git
    cd NetCoreAppWithMicroServices
    ```

2. Restore dependencies and build the services:
    ```bash
    dotnet restore
    dotnet build
    ```

3. Run the services:
    ```bash
    dotnet run --project ProductService
    dotnet run --project OrderService
    dotnet run --project ApiGateway
    ```

### Usage

Access the API Gateway at `https://localhost:5236` to interact with the services. The Swagger UI can be used to test endpoints and view documentation.

### Health Monitoring

MicroNest includes a health check dashboard to monitor the status of each microservice. Access the dashboard at `/dashboard` to see the current status and uptime of each service. The project also integrates with Uptime Robot for continuous monitoring.

## Contributing

Contributions are welcome! Please fork the repository and submit pull requests.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

- Inspired by the principles of microservices architecture and modern web development practices.
- Special thanks to the developers and contributors of the libraries and frameworks used in this project.
