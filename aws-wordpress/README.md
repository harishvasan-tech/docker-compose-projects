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
