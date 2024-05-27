# Unity Shared Services

![Unity Shared Services](https://avatars.githubusercontent.com/u/170880604?s=200&v=4)

**A collection of Shared Unity Services formatted using a simple IService interface**

## Overview

Unity Shared Services is a collection of reusable services designed for Unity projects. Each service adheres to a common `IService` interface, ensuring consistency and ease of integration across different projects.

## Features

- **Modular Architecture**: Each service is a separate package, making it easy to include only the services you need.
- **Versioning**: Services are organized by major versions (`V1`, `V2`, `V3`), ensuring backward compatibility and non-breaking changes.
- **Extensible**: New services can be added seamlessly, following the `IService` interface guidelines.
- **Core Services Included**: Common utilities and services that can be easily extended and customized.

## Getting Started

### Prerequisites

- Unity 2020.3 or later
- Basic knowledge of Unity and C#

### Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourorganization/unity-shared-services.git
    ```
2. Open your Unity project and navigate to `Packages/manifest.json`.
3. Add the local path to the cloned repository:
    ```json
    "dependencies": {
        "com.yourcompany.servicename": "file:../path-to-cloned-repo"
    }
    ```

### Usage

1. Import the required service package in your script:
    ```csharp
    using YourCompany.ServiceName;
    ```
2. Initialize the service:
    ```csharp
    IService service = new ServiceImplementationV1();
    service.Initialize();
    ```

## Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Commit your changes (`git commit -m 'Add YourFeature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a Pull Request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

For any questions or suggestions, please open an issue or contact us at [your-email@example.com](mailto:your-email@example.com).

---

Thank you for using Unity Shared Services! We hope our collection of services makes your Unity development more efficient and enjoyable.
