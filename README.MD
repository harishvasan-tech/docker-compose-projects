# Docker Compose Projects 🐳

A collection of Docker Compose projects built while learning DevOps engineering.
Each project demonstrates multi-container application setup, networking, and volume management.

## Projects

### WordPress + MySQL
A fully containerized WordPress blog with MySQL database backend.

**Services:**
- WordPress (PHP application)
- MySQL 8.0 (database)

**Concepts Demonstrated:**
- Multi-container communication using service names
- Named volumes for database persistence
- Environment variables for configuration
- depends_on for container startup order

**Run it:**
```bash
cd wordpress-mysql
docker compose up -d
```
Access at: http://localhost:8080

---

## WordPress on AWS EC2

Deployed WordPress + MySQL on AWS EC2 using Docker Compose.

**Infrastructure:**
- AWS EC2 t2.micro (Mumbai region)
- Ubuntu 24.04 LTS
- Docker + Docker Compose

**Access:**
- WordPress running on port 8080
- Accessible via public IP

**How to deploy:**
1. Launch EC2 instance
2. Install Docker
3. Run docker-compose up -d
4. Open port 8080 in security group

---

## Concepts Covered
- Docker Compose YAML syntax
- Container networking — service name as hostname
- Named volumes vs bind mounts
- Environment variables in containers
- Container dependency management
- Multi-container debugging

## How to Run Any Project
```bash
# Clone the repo
git clone https://github.com/harishvasan-tech/docker-compose-projects.git

# Go to project folder
cd docker-compose-projects/<project-folder>

# Start containers
docker compose up -d

# Check running containers
docker compose ps

# View logs
docker compose logs

# Stop containers
docker compose down
```

## Tools

- Docker
- Docker Compose
- MySQL
- WordPress
