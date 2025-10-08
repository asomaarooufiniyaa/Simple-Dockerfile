## 🐳 Basic Dockerfile Project

### 🚀 Overview

This project demonstrates how to create a **basic Dockerfile** using the lightweight `alpine:latest` base image.
When the Docker container runs, it simply prints:

```
Hello, Captain!
```

and then exits.

---

### 🧱 Dockerfile Structure

The `Dockerfile` is minimal and easy to understand:

```Dockerfile
FROM alpine:latest
CMD ["echo", "Hello, Captain!"]
```

---

### ⚙️ How to Build and Run

Follow these simple steps to test it locally:

```bash
# 1️⃣ Build the Docker image
docker build -t capitan .

# 2️⃣ Run the container
docker run --rm capitan
```

Expected output:

```
Hello, Captain!
```

---

### 🧩 Optional Enhancement

You can modify the Dockerfile to accept a **build argument** for a custom name:

```Dockerfile
FROM alpine:latest
ARG NAME=Captain
CMD ["sh", "-c", "echo Hello, $NAME!"]
```

Build and run with:

```bash
docker build -t hello-you --build-arg NAME=ASO .
docker run --rm hello-you
```

Output:

```
Hello, ASO!
```

---

### 🏆 Skills Demonstrated

* Creating Dockerfiles from scratch
* Using lightweight base images (Alpine Linux)
* Building and running Docker images
* Using Docker build arguments

---

### 📦 Base Image

* **Image:** `alpine:latest`
* **Purpose:** Small, secure, and fast — ideal for simple Docker experiments and minimal images.

---

### 👨‍💻 Author

**Aso Maarooufiniyaa**
Cloud & DevOps Engineer in training 🌩️
Building the future with automation 🚀


https://roadmap.sh/projects/basic-dockerfile
