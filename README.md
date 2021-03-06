
<i> This repository demonstrates the use of deployment using Github pages for Angular Application . 
The deployed application can be found [here](https://shan7030.github.io/angular-app-github-pages-example/)  </i>

<div style="text-align:center">
<a href="https://shan7030.github.io/angular-app-github-pages-example/"><img src="https://img.shields.io/static/v1?label=&labelColor=505050&message=website&color=%230076D6&style=flat&logo=google-chrome&logoColor=%230076D6" alt="website"/></a>
<a href="https://shan7030.github.io/angular-app-github-pages-example/"><img src="https://img.shields.io/badge/angular-angular--cli%20-red" alt="Angular"/></a>
</div>

<hr>


## Steps for Angular Application Deployment using Github Pages

<ol>
    <li>🚀 Create new Angular Project (You can create one using angular-cli) </li>
    <li>🔨 Now create the web-app according to your need, you can use angular-cli for code scaffolding</li>
    <li>🚀 Create new Repo on Github</li>
    <li>🗃️ Clone the git repo locally using : <br>
      <code> git clone https://github.com/username/reponame.git  </code>
    </li>
    <li> Open terminal/command line (make sure you have git installed), make sure that you are in project directory</li>
    <li> Type the following commands to push the code on github: <br>
      <code>
            git init <br>
            git add . <br>
            git commit -m "Initial Commit" <br>
            git remote add origin https://github.com/username/reponame.git <br>
            git push -u origin master <br>
      </code>
    </li>
    <li> Now, go to github repo and your code should be uploaded to master branch on github </li>
    <li> Next Install the angular-gh-pages using npm: <br>
      <code>npm install -g angular-cli-ghpages</code>
    </li>
    <li> Next, production build the angular application using: <br>
      <code> ng build --prod --base-href "https://username.github.io/reponame/" </code>
    </li>
    <li>Atlast, create the gh-pages branch, also upload the build and bundled code to this branch using : <br>
      <code> ngh --dir dist/reponame </code>
    </li>
    <li>🥵 Now you application is successfully deployed using Github pages</li>
    <li>🚀 You can find the link of deployed application in Settings Tab -> Github Pages </li>
  </ol>

For more detailed steps for installation of angular-cli, git, etc. you can refer <a href="https://www.geeksforgeeks.org/deployment-of-angular-application-using-github-pages/">this</a> article on Geeks for Geeks by me.
