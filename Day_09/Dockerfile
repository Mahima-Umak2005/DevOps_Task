FROM python:3.9-slim

# Create non-root user
RUN useradd -m myuser

# Set working directory
WORKDIR /app

# Copy files
COPY . .

# Give permission
RUN chown -R myuser:myuser /app

# Switch to non-root user
USER myuser

# Run app
CMD ["python", "app.py"]