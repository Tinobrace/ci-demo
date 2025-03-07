# ci/cd-demo

Imagine you’re building a cool toy robot that can do tricks whenever you tell it to. But before it can work, you need to build it, test it, and send it out so your friends can see it in action. That’s exactly what we did with our CI/CD pipeline for deploying a FastAPI app using GitHub Actions, Docker, and Google Cloud. Here’s how it works:

🎯 1. GitHub Actions – The Robot Builder & Tester
Think of GitHub Actions like a team of tiny workers that automatically build, test, and deploy your project whenever you change something. Instead of doing it manually, these little workers follow a set of instructions in a workflow file to get everything ready.

💡 Why?
So we don’t have to build and deploy our app by hand every time—GitHub Actions does it automatically!

📦 2. Docker – The Magic Box for Our App
Imagine you have a toy spaceship, but it needs a special kind of battery, buttons, and lights to work properly. Instead of carrying all these parts separately, you package everything into a single box. That’s exactly what Docker does—it puts our FastAPI app inside a container so it can run anywhere without problems.

💡 Why?
So our app doesn’t break when moving it from one computer to another. Docker makes sure it runs the same way everywhere.

🚀 3. Google Cloud & Artifact Registry – The Toy Store
Now that we’ve built our toy (Docker image), we need a place to store it before sending it out. Think of Google Artifact Registry as a toy store where we keep our packaged app safe.

💡 Why?
So we can easily pull our app from the cloud whenever we want to deploy it.

🔑 4. Service Account & Authentication – The Secret Key
Imagine your toy store has a big lock, and only people with a special key can open it. In our project, we use a Service Account Key (key.json) to prove to Google Cloud that we have permission to upload our app.

💡 Why?
Without this key, Google Cloud won’t let us store or deploy our app. But we must keep it secret so bad people don’t steal it!

🛠 5. CI/CD – The Magic Conveyor Belt
Now imagine you have a conveyor belt that takes your toy spaceship, tests it, packages it, and delivers it to the store automatically whenever you build a new one. That’s exactly what our CI/CD pipeline does—it:
✅ Takes our app
✅ Packages it with Docker
✅ Stores it in Google Cloud
✅ Deploys it automatically

💡 Why?
So we don’t have to do all this work manually. It saves time and prevents mistakes!

🎉 Final Result: A Self-Running Machine!
Now, whenever we update our FastAPI app and push it to GitHub, the pipeline does all the heavy lifting automatically.

No need to build Docker images manually.
No need to push them to Google Cloud ourselves.
No need to worry about deployment breaking.
In Simple Words
1️⃣ GitHub Actions: Auto-builds our app whenever we make changes.
2️⃣ Docker: Puts our app in a container so it runs anywhere.
3️⃣ Google Artifact Registry: Stores our app safely in the cloud.
4️⃣ Service Account Key: Proves we have permission to upload.
5️⃣ CI/CD: Does all of this automatically so we don’t have to!

🚀 Now, we have a fully automated system that takes our code, builds it, and ships it to the world without breaking a sweat. Pretty cool, right? 😎
