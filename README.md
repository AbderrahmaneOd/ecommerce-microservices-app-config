# E-commerce Microservices Configuration Repository

This repository contains the centralized configuration files for the [E-commerce Microservices Application](https://github.com/AbderrahmaneOd/ecommerce-microservices). It serves as the single source of truth for configuration across all microservices, providing a consistent and maintainable approach to application configuration.

## Overview

This configuration repository works in conjunction with the Spring Cloud Config Server to provide externalized configuration for all microservices in the e-commerce application. By centralizing configuration, we can:

- Maintain configuration consistency across environments
- Update configuration without rebuilding applications
- Support environment-specific configuration properties
- Version control all configuration changes

## Repository Structure

The repository is organized by service name and profile:

```
ecommerce-microservices-app-config/
├── api-gateway.yml                 # Default config for API Gateway
├── api-gateway-docker.yml          # Docker-specific config for API Gateway
├── discovery-server.yml            # Eureka server configuration
├── inventory-service.yml           # Inventory service configuration
├── inventory-service-docker.yml    # Docker-specific config for Inventory
├── notification-service.yml        # Notification service configuration
├── notification-service-docker.yml # Docker-specific config for Notifications
├── order-service.yml               # Order service configuration
├── order-service-docker.yml        # Docker-specific config for Orders
├── product-service.yml             # Product service configuration
├── product-service-docker.yml      # Docker-specific config for Products
├── user-service.yml                # User service configuration
└── user-service-docker.yml         # Docker-specific config for User service
```

## Configuration Profiles

The repository contains configurations for different profiles:

- **Default**: Base configuration for all environments
- **Docker**: Specific configuration for containerized deployment