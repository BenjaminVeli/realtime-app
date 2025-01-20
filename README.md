### Realtime Chat App

<a href="https://www.youtube.com/watch?v=ntKkVrQqBYY&t=13834s" target="_blank">Creator burakorkmez</a>

## MERN Stack Project:

- **Database**: MongoDB for storing user and chat data.
- **Frontend**: ReactJS for the interface, styled with TailwindCSS and DaisyUI for modern UI components.
- **Backend**: Express.js API for server-side logic, utilizing JWT for authentication and authorization.
- **Realtime Messaging**: Socket.io is used for instant communication and real-time updates.
- **State Management**: Zustand for global state management to handle app-wide state efficiently.
- **Image Management**: Cloudinary is integrated for image uploads and management.

## Prerequisites:

- **Node.js**
- **Cloudinary** account for image storage
- **MongoDB Atlas** account for data storage
- **Docker (optional)** for running MongoDB in containers

### Initialize Backend :

**If using MongoDB Atlas**, refer to this video at minute 14:04:  
[How to set up MongoDB Atlas](https://www.youtube.com/watch?v=ntKkVrQqBYY&list=LL&index=1&t=63s)

**Create account Cloudinary**, refer to this video at minute 1:02:24:  
[How to create an account on Cloudinary](https://www.youtube.com/watch?v=ntKkVrQqBYY&list=LL&index=3&t=63s))

### Steps to set up MongoDB with Docker:

1. Pull the MongoDB Docker image:
   ```sh
   docker pull mongo
   ```
2. Create MongoDB container::

   ```sh
   docker create -p27017:27017 --name mongocontainer -e MONGO_INITDB_ROOT_USERNAME=root -e MONGO_INITDB_ROOT_PASSWORD=password mongo
   ```

3. Run MongoDB container::

   ```sh
   docker start mongocontainer
   ```

4. Verify the container is running::
   ```sh
   docker ps
   ```

```sh
cd backend
mv .env.example .env
npm install
npm run dev
```

### Initialize Frontend :

```sh
cd frontend
npm install
npm run dev
```
