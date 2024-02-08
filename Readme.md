# Project Name

Description of your project.

## Table of Contents

- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
- [Folder Structure](#folder-structure)
- [Tech Stack](#tech-stack)
- [Contributing](#contributing)
- [License](#license)

## Getting Started

### Prerequisites

- [Docker](https://www.docker.com/) - Ensure you have Docker installed.

### Installation

1. Clone the repository:

```bash
git clone https://github.com/poroto82/QuoteStack.git --recurse-submodules 
cd QuoteStack
```
Set up environment variables:

Create .env file in the root of the Laravel project based on .env.example.

Configure Laravel database settings.
Build and run the Docker containers:

```bash
docker-compose up --build
```
Install Laravel dependencies:
```bash
docker-compose exec quote-back composer install
```
Migrate and seed the database:
```bash
docker-compose exec quote-back php artisan key:generate

docker-compose exec quote-back php artisan migrate --seed

docker-compose exec quote-back php artisan passport:install

```


Folder Structure
Briefly explain the structure of your project's folders and key files.

Tech Stack
Laravel
React
Nginx
Docker
List other technologies and frameworks used in your project.

Contributing
If you'd like to contribute, please follow the Contributing Guidelines.