# Docker Compose with Nginx Load Balancing

This repository contains the necessary configuration files to deploy a multi-instance application using Docker Compose and Nginx for load balancing.

## Structure

- `docker-compose.yml`: Docker Compose file that defines the application and Nginx services.
- `nginx/`: Directory containing the Nginx configuration file.
  - `nginx.config`: Nginx configuration file that sets up the load balancing between application instances.

## Usage

1. Clone this repository.
2. Replace `your_application` with the name of your application in the `docker-compose.yml` file.
3. Modify the `nginx.config` file to match the IP address and port numbers of your application instances.
4. Run `docker-compose up` to start the application and Nginx services.
5. Access the application via the exposed port on the Nginx service (default: `5000`).

## Customization

- Adjust the number of replicas in the `docker-compose.yml` file to control the number of application instances.
- Update the `nginx.config` file to add or remove application instances as needed.
- Modify the exposed ports in the `docker-compose.yml` file to match your desired setup.

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for more information.

