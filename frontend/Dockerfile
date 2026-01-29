FROM node:20

WORKDIR /usr/src/app

# Copy dependency files
COPY package*.json ./

# Install dependencies cleanly
RUN npm install

# Copy the rest of the source code
COPY . .

# Expose the Vite dev server port
EXPOSE 5173

# Run Vite dev server and bind to all interfaces
ENV TMPDIR=/tmp
CMD ["npm", "run", "dev", "--", "--host", "0.0.0.0"]
