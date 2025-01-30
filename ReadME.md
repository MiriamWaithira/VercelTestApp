## Create a Node.js Project ##
1. Create a directory named VercelTestApp and navigate into the directory using VSCode.
2. Open terminal (git bash) and initialize the node.js project using the command "npm init -y". This will create the 'package.json' file.
3. Install Express.js (a popular node.js framework) using the command "npm install express". This will create 'package-lock.json' file and 'node_modules' directory.
4. At the root of your folder, create 'index.js' file and write the code as in the file.
5. At the root of your folder, create '.gitignore' file, open it and write 'node_modules/' inside it and any other file you want ignored as it is being pushed to github.
6. To run the server:
    1. type in the terminal 'node index.js'
    2. Or navigate to the package.json file and add the line '"start": "node index.js"'under scripts. This way, you only need to type 'npm start' to run the server.

## Configuring Vercel ##
1. Create a 'vercel.json' file at the root directory of your project and add content as it is in the file.

## Pushing to github ##
1. Create a new repository in your github account named VercelTestApp.
2. Go back to your terminal and type in the following commands:
    1. git init
    2. git add .
    3. git commit -m"Initial Commit"
    4. git branch -M main
    5. git remote add origin https://github.com/your-username/VercelTestApp.git
    6. git push
    7. git push --set-upstream origin main
Once you reload the github repository, the file will have been uploaded.

## Deploying to Vercel ##
1. Log in to your Vercel account (or create a new account if you dn't  already have one) and navigate to your dashboard.
2. Click on “New Project” and import the GitHub repository you just created.
3. After importing, configure any necessary settings (most likely, you won’t need to change anything. If you have any .env file files please add them where necessary.).
4. Click on “Deploy.”
5. Once deployment has finished, click 'Continue to dashboard', then click on the link below 'domains'. The server works perfectly.