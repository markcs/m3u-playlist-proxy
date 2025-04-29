# What is the M3U Playlist Proxy

The M3U Playlist Proxy is a lightweight and effective tool designed to forward essential headers to proxy M3U playlist streams. Acting as a bridge between your client and the server, it ensures that important headers (such as User-Agent, Referer, etc.) are accurately passed along. This setup allows IPTV applications to reliably access streams that need specific headers in place.

**Formats Supported:** The M3U Playlist Proxy supports Standard, TiviMate, Kodi, and VLC M3U formats. You can now use any of these formats when loading playlists into MPP.

## Deploy to Vercel

Vercel’s free tier includes 100 GB of bandwidth and 1,000 build minutes per month, making it an excellent option for deploying the m3u-playlist-proxy. This allocation is more than enough to manage personal stream proxying and development needs efficiently.

https://github.com/user-attachments/assets/4fd3c242-b1d0-4f2b-bccb-d0b98b8ba94e

Click the button below to deploy this project to Vercel.

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/import/project?template=https://github.com/markcs/m3u-playlist-proxy)

### Steps to Deploy:

1. **Click the Deploy Button**:
- When you click the **Deploy with Vercel** button, you'll be redirected to Vercel's platform. It will automatically import the project template from this GitHub repository.

2. **Log in Using GitHub**:
- It is recommended to log in to Vercel using a GitHub account. This makes the integration smoother and allows Vercel to access the repository directly. If you don’t have a Vercel account, you can sign up for free.

3. **Configure Project Settings**:
- After logging in, Vercel will guide you through the project setup. You can review the project name and select the team or personal account under which you want to deploy the project.

4. **Deploy the Project**:
- After confirming the settings, click **Deploy**. Vercel will automatically build and deploy the project based on the configuration defined in the repository.

5. **View the Live Project**:
- Once the deployment is complete, you will see a link to access your newly deployed project.

   **IMPORTANT**

   If you click the link directly and receive a 400 Bad Request error, this may be due to a `?vercelToolbarCode=xxxxxx` parameter being added to the URL. Simply remove this parameter from the address bar and reload the page.

## Setup with Docker

The M3U Playlist Proxy is also available as a Docker image, allowing you to easily deploy it in a containerized environment. By using Docker, you can quickly start the proxy without needing to install dependencies or manually configure the environment.

### Pulling the Docker Image

To get started, pull the latest version of the M3U Playlist Proxy Docker image with the following command:

`docker pull dtankdemp/m3u-playlist-proxy:latest`

### Running the M3U Playlist Proxy Container

Once you’ve pulled the image, you can start the container using:

`docker run -d -p <port>:4123 dtankdemp/m3u-playlist-proxy:latest`

This command runs the proxy on port 4123, allowing your IPTV application to connect to it locally or remotely (depending on your setup) to access M3U playlist streams with the necessary headers correctly forwarded. Adjust the port if needed, based on your environment.
