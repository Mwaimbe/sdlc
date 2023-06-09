
Project Name : <PROJECT_NAME>
VS code shortcuts
react functional component
rfc

# STAGE 4 : CODING AND IMPLEMENTATION

## Building Blocks of a Web Application

1. User Interface
   How users will consume and interact with your application.
   React, Tailwind,Formik,Yup,Django (Admin),React-toastify,primereact,plotly js
   https://react.dev/
   https://tailwindcss.com/
   https://primereact.org/
   https://plotly.com/javascript/getting-started/

2. Routing
   How users navigate between different parts of your application.
   Next js 13 (stable)
   https://nextjs.org/

3. Data Fetching
   Where your data lives and how to get it.
   Next js, Prisma,GraphQL

4. Rendering
   When and where you render static or dynamic content
   Next js

5. Integrations
   What third-party services you use (CMS, auth, payments, etc) and how you connect to them.
   NextAuth js,Twilio

6. Infrastructure
   Where you deploy, store, and run your application code (Serverless, CDN, Edge, etc)
   AWS,Github

7. Performance - how to optimize your application for end-users.
8. Scalability - how your application adapts as your team, data, and traffic grow
9. Developer Experience - your team’s experience building and maintaining your application.



## Setup
https://nextjs.org/docs/getting-started

```bash
npx create-next-app@13.3.1
```
or 
```bash
npx create-next-app@latest
```

√ What is your project named? ... <project_name>
√ Would you like to use TypeScript with this project? » No
√ Would you like to use ESLint with this project? » Yes
√ Would you like to use Tailwind CSS with this project? » Yes
√ Would you like to use `src/` directory with this project » No
√ Would you like to use experimental `app/` directory with this project?  » No
√ What import alias would you like configured? ... @/* 


## git/github

Install git 

https://git-scm.com/downloads

Configuration

```bash

git config --global user.name <Your-name>
git config --global user.email <your_email>

```

version

```bash

git -v

```

#### git and github workflow

Git is a distributed version control system used to track changes in software code over time. GitHub is a web-based hosting service for Git repositories. GitHub allows users to collaborate on projects, share code, and contribute to open-source projects.

Here is a typical workflow for using Git and GitHub:

Create a new repository:
Create a new repository on GitHub or use the Git command line to create a new local repository.

Clone the repository:
Clone the repository to your local machine using the Git command line.

Make changes to the code:
Make changes to the code on your local machine using your preferred code editor.

Stage changes:
Use the Git command line to stage the changes you want to commit.

Commit changes:
Use the Git command line to commit the staged changes with a commit message that briefly describes the changes.

Push changes:
Use the Git command line to push the committed changes to the remote repository on GitHub.

Review changes:
Review changes in the GitHub interface or using Git command line tools.

Pull changes:
If other team members have made changes to the code, use the Git command line to pull those changes to your local machine.

Resolve conflicts:
If there are conflicts between your changes and changes made by other team members, use the Git command line to resolve the conflicts.

Repeat:
Continue making changes, staging, committing, and pushing to the repository, collaborating with other team members using Git and GitHub.

This workflow is just an overview and there are many more advanced features and commands that can be used in Git and GitHub. It's also important to follow best practices, such as making small, frequent commits with descriptive commit messages, and regularly pulling changes to ensure everyone is working with the latest code.



git status

```bash

git status

```

git init - Create an empty Git repository or reinitialize an existing one in the current directory

```bash

git init .

```

git add - Add all existing files to the index

```bash

git add .


```

git add <file>
Add specified file to the index/staging to prepare for commit

```bash

git add <file>

```

git rm --cached <file> 
Unstage

```bash
git rm --cached <file>

```



git commit -m "initial commit" 
Record the pristine state as the first commit in the history

``` bash

git commit -m "initial commit"

```
git commit - opens the editor

```bash
git commit

```

git commit -a 
Express commits to a repository without staging. -a stands for all. All changes are committed.Opens the editor. remmoves any deleted files from the commit.Untracked files will not be added
opens default editor

```bash
git commit  -a 

```

git commit -am "message"
Express commit
```bash
git commit  -am "your commit message"

```

Git states

Working directory > Staging area >Repository (.gitfolder)


1. git add <file> or git add .
2. git commit -m "initial commit"
3. 

rm -rf .git
remove/delete .git folder

```bash
rm -rf .git

```
rm <file>
remove file.Permanently deleted
You also need to commit
```bash
rm <file>
```

rm -r <dir>
remove the directory specified with all its files and subdirectories
You also need to commit
```bash

rm -r <dir>

```

git log
commit history
If you see "(END)" at the bottom of the screen, it means that you have reached the end of the Git log. To exit, simply press the "q" key.

```bash

git log

```

git log --oneline 

```bash

git log --oneline

```

git log --oneline --graph
```bash

git log --oneline --graph

```


git checkout -- <file>
discard changes made to a file that has not been staged
Contents replaced with content that is currently stored in the git repository
This will replace the contents of the file with the last committed version in the Git repository, effectively undoing any changes made to the file.

```bash 
git checkout -- <file>

```

git checkout <file>
used to switch to a different version of the file from a different branch or commit.
 running "git checkout <file>" without specifying a branch or commit will result in detaching the HEAD and checking out a "dangling" commit. This can result in data loss and should be avoided.



git checkout <hash>

```bash

git checkout 0a7b7b7

```
If you want to go to a specific commit in a Git repository, you can use the git checkout command followed by the commit hash or branch name. For example, if you want to go to a commit with the hash abc123, you can run the command git checkout abc123. This will switch your working directory to the state of the repository at that commit.

If you want to see the changes made in a specific commit, you can use the git show command followed by the commit hash. For example, if you want to see the changes made in the commit with the hash abc123, you can run the command git show abc123.

Note that making changes to the repository while in a specific commit state can result in a detached head state, so be careful when working with commits in this way.

error: Your local changes to the following files would be overwritten by checkout:
        Stage 4 -  Coding and Implementation.md
Please commit your changes or stash them before you switch branches.
Aborting

















git reset -- hard HEAD
Undo all changes made to the repository since the last commit

```bash 
git reset -- hard HEAD

```
git reset HEAD <file>
unstage changes to a file that have been added to the staging area in Git.

```bash 
git reset HEAD <file>
```
 git restore <file>
 To discard changes in working directory

 ```bash 
 git restore <file>
 ```
 (use "git restore --staged <file>..." to unstage)

 git reset HEAD <file>
to unstage

git mv <old_file> <new_file>
rename file
You also need to commit

```bash 
git mv <old_file> <new_file>

```

git add -A
git add -u



git diff

git difftool



HEAD
Points to the last commit of the current branch



git branch
See the branches
```bash
git branch
```
git branch -a

```bash
git branch -a
```


git checkout -b  <new_branch>
create a new branch
```bash
git checkout -b new_feature
```

git checkout <branch>
switch to a specified branch

```bash
git checkout <branch>

```



git merge <branch_you_want_to_merge_to_the_main>
first switch to the parent branch e.g main/master using the git checkout main command

you need to stage and/or commit all

```bash
git merge <branch_you_want_to_merge_to_the_main>

```

git branch -d <branch>
deletes a branch

```bash
git branch -d <branch>
```

git push origin :<branch>
deletes a remote branch
```bash
git push origin :admin
```


conflict resolution

handling file updates/changes in both branches

```bash

<<<<<<< HEAD
still on the main branch
=======
conflict resolution - bad branch
>>>>>>> badbr

```

## Tags

https://absagroup.udemy.com/course/github-ultimate/learn/lecture/4732050#overview

git tag -a <tag_name> -m "<message>" <hash>

```bash
git tag -a v1.0 -m "Release 1.0" d4112ew
```

git tag --list
```bash
git tag --list
```

git push origin <tag_name>


git push  --tags

## update tags  floating tags

git tag -f <tag_name> <hash>

git push  --force origin <tag_name>

#### multiple remote
git remote add origin <url1>
git remote add upstream <url2>

you can use
git fetch --all


## Releases



stable
v0.1-alpha
v0.5-beta
Release 1.0




stashing
git stash
git stash pop


git reset <hash> --soft | mixed | hard


git reflog


To use autocomplete in Git Bash, you can either press the "Tab" key to complete the command or filename, or press the "Tab" key twice to display a list of possible completions.





Use the imperative mood: Start your commit message with a verb in the imperative mood (e.g. "Add", "Fix", "Update", "Remove"). This helps to make your message more actionable and clear.

Be specific: Include enough detail in your commit message so that others can understand what changes you made and why. If your commit relates to a particular issue or feature, reference it in the message.

Separate subject from body: If your commit message needs more detail, separate the subject from the body with a blank line. The subject should be a brief summary of the change, while the body should provide more context and information.


```bash
Add new feature to search bar

This commit adds a new autocomplete feature to the search bar, allowing users to quickly find and select search terms.


Update error handling for login page

This commit updates the error handling for the login page, providing more detailed error messages and better user feedback.


Remove deprecated code from API

This commit removes deprecated code from the API, reducing complexity and improving performance.

Fix bug in checkout process

This commit fixes a bug that caused the checkout process to fail when certain items were added to the cart.


Refactor code for better readability

This commit refactors the code to improve readability and maintainability, simplifying complex logic and removing unnecessary comments.



Fix typo in README.md

The word "commmit" was misspelled in the README. This commit corrects the typo to improve clarity.

```


https://absagroup.udemy.com/course/github-ultimate/
https://absagroup.udemy.com/course/git-and-github-bootcamp/learn/lecture/24507864#overview






settings


git/github workflow

1. create a github repo - should match local repo, should be empty
2. Link a local repository to the github repo
3. Push to the remote repo

git remote -v
Show the current list of remote repositories that are connected to your local Git repository. The -v option stands for "verbose" and is used to display more detailed information about each remote repository.

```bash 
git remote -v
```

git remote add <name> <url>
-- adds origin
```bash
git remote add origin https://github.com/Mwaimbe/sdlc.git
```
or - adds upstream 
```bash
git remote add upstream https://github.com/Mwaimbe/sdlc.git
```

git remote rm origin
```bash
git remote rm origin
```

git push -u origin main


```bash
git push -u origin main
```

git remote remove <name>
```bash
 git remote remove Mwaimbe/napa

```

git remote set-url origin <new url>
```bash
git remote set-url origin git@github.com:Mwaimbe/sdlc.git

```

SSH keys
SSH or Secure Shell is a network communication protocol that enables two computers to communicate


local
create dir ssh
use vs code
```bash
ssh-keygen -t rsa -C "<your email>"
```
Enter file.... <Enter>
Enter passphrase <recomended>

Your identification has been saved in /c/Users/hp/.ssh/id_rsa
Your public key has been saved in /c/Users/hp/.ssh/id_rsa.pub



show the file

```bash
ls -al

```
public
copy file contents of id_rsa.pub

verify ssh

```bash

ssh -T git@github.com
```


git clone <url> <dirname>
Create a local copy
<dirname> optional - Name of the folder to be created and files copied to

```bash
git clone git@github.com:The-shark/OneOffTransactions.git oneofftransactions
```



git fetch
Download contents from a remote repository
git fetch is a Git command that retrieves changes from a remote repository without integrating them into the local branch. It is useful for keeping the local repository up-to-date with the changes made in the remote repository.

When you run git fetch, Git retrieves the latest changes from the remote repository and updates the remote tracking branch, which is a local reference that tracks the state of the remote repository. This allows you to see the changes made in the remote repository without modifying your local branch.

After running git fetch, you can review the changes made in the remote repository using tools like git diff or git log. If you want to integrate the changes into your local branch, you can use commands like git merge or git rebase.

Note that git fetch only retrieves changes from the remote repository, it does not modify any of your local files. To update your local files with the changes from the remote repository, you need to run additional commands such as git merge or git rebase.


```bash
git fetch
```

git fetch -p
Remove any references to non existent branches

```bash
git fetch -p
```

git pull
update your local branch from a remote repository
Preferrable

```bash
git pull
```


git push
```bash
git push
```

git push --set-upstream origin revised
```bash
git push --set-upstream origin revised
```

pull requests
Pull requests let you tell others about changes you've pushed to a branch in a repository on GitHub. 
Once a pull request is opened, you can discuss and review the potential changes with collaborators and add follow-up commits before your changes are merged into the base branch.

Mwaimbe wants to merge 3 commits into development from revised



fork
A fork is a new repository that shares code and visibility settings with the original “upstream” repository. 
Forks are often used to iterate on ideas or changes before they are proposed back to the upstream repository, such as in open source projects or when a user does not have write access to the upstream repository.



In the context of version control systems like Git, a fork and a clone refer to two different concepts:

Fork: A fork is a copy of a repository in a version control system, typically hosted on a different platform or account. When you fork a repository, you create your own copy of it that you can modify independently of the original. This is often used when you want to contribute to someone else's project on a hosting platform like GitHub, but don't have direct write access to the original repository.

Clone: Cloning a repository means creating a local copy of it on your own computer. When you clone a repository, you download a complete copy of all the files and history associated with that repository. This allows you to work on the code or files locally, make changes, and then push those changes back up to the original repository or to your own fork.

In summary, while both fork and clone create copies of a repository, a fork creates a new independent copy on a different platform or account, while a clone creates a local copy on your own computer.



github
go to the project you want to fork 
fork

go to your account and clone
```bash
git clone git@github.com:The-shark/CarBid.git
```

local
create your own branch

git checkout -b <newfeature>

---make your contributions---

push
```bash
git push -u origin newfeature
```

 Create pull request
 on github click on compare and pull request or Contribute

accept pull request
-done on github

synchronise changes back to your fork
git pull origin <branch>
```bash
git pull origin master
```

enlist help with collaborators


rebase
The git rebase command allows you to easily change a series of commits, modifying the history of your repository. You can reorder, edit, or squash commits together. Typically, you would use git rebase to: Edit previous commit messages. Combine multiple commits into one.

```bash
git pull --rebase
```

## pull request

merge

issuesu

gists


ls -l

cd <dir>
cd ..


git mergetool
conflict while pulling
```bash
git mergetool
```

default branch
- 

branches
- main
- develop
        - new feature
        - theme


collaborators
have full access
repo > settings > collaborators



  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)

### Issue tracking

git hub

Issues are used to track todos, bugs, feature requests, and more. As issues are created, they’ll appear here in a searchable and filterable list. To get started, you should create an issue.

labels
milestones

##### Associating issues with commits
Issue: Sidebar overflow hover distortion #2


```bash
git commit -m 'Sidebar hover distortion,close #2'
```
then push to github

@Mwaimbe Mwaimbe closed this as completed in 48e8c60 8 minutes ago


#### Gist
In GitHub, a "gist" is a simple way to share code snippets, notes, and other small pieces of text with others. It allows you to quickly and easily create and share snippets of code without having to create a full-fledged repository.

Instantly share code, notes, and snippets.




##### local gist
git clone git@gist.github.com:fefa2b5b54f0f4d5943ae8b08c0f6d71.git <name>
```bash
git clone git@gist.github.com:fefa2b5b54f0f4d5943ae8b08c0f6d71.git palletes
```

##### sharing gists

use url



### github organizations










## Imports
To make use of path alias,configure the jsconfig.json

https://dev.to/rhammy/path-aliases-in-nextjs-2fnc

Example

```json
{
  "compilerOptions": {
    "baseUrl":".",
    "paths": {
        "@/*": ["./*"],
        "@/components/*":["./components/*"],
        "@/context/*":["./context/*"],
    }
  }
}
```

## Layouts
https://nextjs.org/docs/basic-features/layouts

Single Shared Layout

Create a layout component

``` javascript
// components/Layout.jsx
import SideBar from './SideBar'
import NavBar from './NavBar'
export default function Layout({children}) {
  return (
    
    <div className="flex flex-row">
          <div className="w-44 bg-slate-50 border-r-2 border-neutral-100 h-screen fixed overflow-y-auto px-2">
            <SideBar />
          </div>
          <div className="flex flex-col flex-grow ml-44">
            <section className="z-10 grow fixed top-0 bg-white shadow py-1 px-1 w-[calc(100%_-_11rem)]">
              <NavBar />
            </section>
            <section className="flex flex-row py-16  px-8">
                {children}
            </section>
          </div>
        </div>
  )
}


```

``` javascript
// pages/_app.js
import NewProductContextProvider from '@/context/NewProductContext'

import Layout from '@/components/Layout'
export default function App({ Component, pageProps }) {
  return (
    <Layout>
    <NewProductContextProvider>>
      <Component {...pageProps} />
      </NewProductContextProvider>
    </Layout>
  )
}


```
## pages
In Next.js, a page is a React Component exported from a .js, .jsx, .ts, or .tsx file in the pages directory. 
Pages must be named with lower case
The component should be exported as the default export of the file.
The name of the page component doesnt really matter but must be exported as default
index.js is the root path



``` javascript
// 
// If you create pages/new/index.js that exports a React component like below, it will be accessible at /new.

export default function Form() {
  return (
    <div>
        Form
    </div>
  )
}

```


## next/head
The contents of head get cleared upon unmounting the component, so make sure each page completely defines what it needs in head, without making assumptions about what other pages added.

``` javascript
import Head from 'next/head'

export default function Page() {
  return (
    <div>
       <Head>
        <meta charSet="utf-8" />
        <title>NAPA</title>
        <meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover" />
        <meta name="description" content="Description......." />
        <meta name="keywords" content="webdev, javascript, beginners, react, software, coding, development, engineering, inclusive, community" />
      </Head>
      <p>Hello world!</p>
    </div>
  )
}

```

## next/link
Client-side transitions between routes can be enabled via the Link component exported by next/link.

Link accepts the following props:

href - The path or URL to navigate to

as - Optional decorator for the path that will be shown in the browser URL bar.

## File-based routing
Each page is associated with a route based on its file name

Next.js has a file-system based router built on the concept of pages.

When a file is added to the pages directory, it's automatically available as a route


## Dynamic Routes
You can add brackets to a page ([param]) to create a dynamic route (a.k.a. url slugs, pretty urls, and others).

pages/post/[pid].js

``` javascript
import Link from 'next/link'
export default function Home() {
  return (
    <div>
         <ul>
            <li>
                <Link href="/">Home</Link>
            </li>
            <li>
                <Link href="/about" as="Lorem Ipsum">About Us</Link>
            </li>
            <li>
                <Link href="/blog/[slug]" >Blog Post</Link>
            </li>
        </ul>
    </div>
  )
}

```

## Navigating programatically

-   useRouter hook
-   When an event is triggered/completed
-   router.push('/') --- takes you to the homepage
-   router.replace('/')
-   useRouter is a hook provided by the next/router module in the Next.js framework.
-   It allows you to access the router object, which you can use to programmatically 
    navigate between pages in your Next.js application.
-   Can only be used within a functional component or a custom hook.
-   useRouter returns an object
-   Add active class
-   
  ```javascript
      className={`${router.pathname === '/' ? 'active' :''} flex flex-row items-center h-10`}
  ```


## 404 - Page Not Found

- add 404.js in the pages folder


## forms
Formik
Formik is the world's most popular open source form library for React and React Native.
https://formik.org/

## form validation
Yup


## form api route















## api routes

-   API routes provide a solution to build your API with Next.js
-   Any file inside the folder pages/api is mapped to /api/* and will be treated as an API endpoint instead of a page.
-   They are server-side only bundles and won't increase your client-side bundle size.
-   API Routes do not specify CORS headers, meaning they are same-origin only by default.3
-   Cross-Origin Resource Sharing (CORS) is an HTTP-header based mechanism that allows a server to indicate any origins (domain, scheme, or port) other than its own from which a browser should permit loading resources. 
-   API Routes can't be used with next export




## Styling

tailwind


#### TeXT Editor


https://primereact.org/editor/






## Components

https://primereact.org/


## Tables



DataGrid
https://mui.com/material-ui/react-table/

https://mui.com/x/react-data-grid/events/



#### Graph
https://plotly.com/javascript/getting-started/

npm install react-plotly.js plotly.js


---
## Caching
---


---
## Forms
---

- Form components
- Form handling
Formik
https://formik.org/

- Form validation
yup

- Multi-step form

Resources
https://www.youtube.com/watch?v=oPteQFUK42w
https://www.youtube.com/watch?v=l3NEC4McW3g
https://formik.org/docs/guides/validation

https://www.youtube.com/watch?v=xAjbUJfpoz0


Stepper - 
https://flowbite.com/docs/components/stepper/

Material ui stepper



### value binding
- bind values set in the state
input value={value}


---
## Filtering data
---
filter()
find()


---
## Media
---
- File upload

import Dropzone from "react-dropzone";



---
## ICONS
---
react-icons

https://react-icons.github.io/react-icons/icons?name=fa

https://mui.com/material-ui/icons/

npm install @mui/icons-material





https://mui.com/material-ui/getting-started/overview/

---
## CONNECTING & WORKING WITH THE DATABASE
---
1. Prisma -ORM
2. MS SQL/MySQL,PostGre
3. GraphQL
4. AWS Amplify 





#### Prisma 
- Prisma is an open-source ORM that drastically simplifies data modeling, migrations, and data access for SQL databases in Node.js and TypeScript.
- Object Relational Mapping (ORM) is a technique used in creating a "bridge" between object-oriented programs and, in most cases, relational databases

dependencies

npm i -D  prisma
npm i @prisma/client
npx prisma init



--- prisma studio
npx prisma studio

   npx prisma db push



### Connection
-  Create one instance of PrismaClient and re-use it across your application




https://www.prisma.io/docs/getting-started/setup-prisma/start-from-scratch/relational-databases/using-prisma-migrate-node-sqlserver


## is owner policy
- The owner is the person who created a record
- If true , only they can perform actions on the record
- If false , anyone
- If hybrid, they and designated users

 
https://www.prisma.io/docs/getting-started

        Prisma Client requires TCP/IP to be enabled. To enable TCP/IP:

Query data from MySQL, PostgreSQL & SQL Server databases in Next.js 





#### AWS Amplify
- Data storage
- Authentication
- File storage
- Hosting
- AI and ML
- 

Amplify cli
npm install -g @aws-amplify/cli
amplify configure




---
## PAGE RENDERING STRATEGY
---

1. Client side rendering
2. Server side rendering

The main difference between CSR and SSR is where the page is rendered. SSR renders the page on the server-side and CSR renders the page on the client-side.

### Client side rendering (CSR)
- Client-side using useEffect hook or useQuery - data updated at evry request
- Client side + api route suing useEffect + api handler -- data fetched on client at evry request
   
### Server side rendering (SSR)
- Static generation using getStaticProps -- Data fetched at build time
- Incremental static generation using getStaticProps + revalidate -- Data fetched at build time and updated every x seconds [***]
- Server-side rendering using getServerSideProps -- data fetched on server at run time updated at every request

    ##### getServerSideProps 
    -   Allows you to fetch data from a backend or an external API during server-side 
        rendering. 
    -   data fetched in this function is used to generate the HTML content of the page on 
        the server before it is sent to the client. 
    -   This can improve performance and SEO, as search engines can crawl the fully rendered page.

```javascript
    // MyPage.js

    export async function getServerSideProps(context){
        // fetch data
        const res = await fetch(url)
        const data = await res.json()
        return {
            props: { data }
        }
    }

    function MyPage({data}){
        return (
            <div>
                { data }
            </div>
        )
    }
```

-   In this example, the getServerSideProps function fetches data from an external 
    API and returns it as props to the MyPage component. 
-   The data prop is then used to render the page content.

#####  getStaticPaths & getStaticProps
- Renders pages at build time




---
## DATA FETCHING STRATEGY 
---
1. React Query
2. fetch
3. axios
4. swr

#### React Query
- React Query is a ReactJS preconfigured data management library which gives you power and control over server-side state management, fetching, and caching of data, and error handling in a simple and declarative way without affecting the global state of your application.
- useQuery is a hook provided by the React Query library that makes it easy to fetch and manage data in a React component. getStaticProps is a Next.js function that enables server-side rendering for a page by fetching data during build time.
- https://www.youtube.com/watch?v=r8Dg0KVnfMA
- 
npm install react-query

### swr
##### get request

### post /put / delete request

##### Data post/put/delete strategy 



##### fetch 


### Skeleton loading div
https://www.section.io/engineering-education/skeleton-loading-in-nextjs-with-tailwindcss/




#### Loading/Progress
https://www.npmjs.com/package/nextjs-progressbar

npm i nextjs-progressbar

```javascript
//pages/_app.js

import NextNProgress from 'nextjs-progressbar';

export default function MyApp({ Component, pageProps }) {
  return (
    <>
      <NextNProgress color="#ff0000" />
      <Component {...pageProps} />;
    </>
  );
}

```

#### Fallback: blocking
- getStaticPaths




## Unique id
1. cuid
2. uuid
3. crypto.randomUUID()


### api routes

---
## API
---
- GraphQL
- GraphQL is a query language for APIs and a runtime for fulfilling those queries with your existing data. GraphQL provides a complete and understandable description of the data in your API, gives clients the power to ask for exactly what they need and nothing more, makes it easier to evolve APIs over time, and enables powerful developer tools.

---
## STATE MANAGEMENT
---
1. Redux
2. useState hook
3. useContext hook
4. Persisting State in React Apps


-   Redux, useState, and useContext are all tools in React for managing state. 
-   Each has its strengths and weaknesses, and which one you should use depends
    on the specific needs of your application.

##### redux
-   Redux is a state management library that provides a global store for managing 
    application state
-   It allows for a predictable state container and provides a single source of truth
    for your application's data
-   It is useful for managing complex data and for sharing state between components. 
-   However, it can add complexity to your codebase, and it may not be necessary for 
    smaller applications.

##### useState
-   useState is a built-in React hook that allows you to add state to your
    functional components.
-   It is simple to use and doesn't require any additional libraries. 
-   It is a good choice for managing simple state that is only needed within 
    a single component.

##### useContext
-   useContext is another built-in React hook that allows you to share state between 
    components without the need for props drilling. 
-   It is useful when you need to share state between multiple components that are not
    directly related to each other.

    Make persistent ?? localStorage












-   In summary, if you have a large, complex application with many components that need 
    to share state, Redux is a good choice. If you have a smaller application or 
    only need to manage simple state within a component, useState may be sufficient. 
    If you need to share state between multiple components, useContext may be the 
    best option.













## Themes
https://www.youtube.com/watch?v=Uz35Qiia84g



## Error Handling

### Messaging

### Emails
npm install nodemailer
## NOTIFICATION
- React-toastify
- https://fkhadra.github.io/react-toastify/introduction/












## Authorization and access control
## Storing HttpOnly Cookies on the server



## Refactoring

## Fallback and Backend unavailable
-- Display static pages


## Environement variables
.env 
.env.local


### Components
 react components




### Back end code
    - use node js



Hydration





--------------------------------------------------------
React animations
--------------------------------------------------------
-  https://www.framer.com/motion/?utm_source=google&utm_medium=adwords&utm_campaign=TW-WW-All-GS-UA-Traffic-20190326-Brand.Bmm_

-   

---
## TESTING
--- 
1. E2E
2. Unit Tesiting



---
## AUTHENTICATION AND AUTHORIZATION
---
- Authentication is the act of proving an assertion, such as the identity of a computer system user
- Authorization or authorisation is the function of specifying access rights/privileges to resources


1. Sign up
2. Sign in
3. Sign Out
4. Page access
5. Page content access


### next-auth
- https://next-auth.js.org/
- https://www.youtube.com/watch?v=bLlDwkOyI5c
- 

Technology used
NextAuth.js
https://next-auth.js.org/

JWT
-   It is a compact, URL-safe means of representing claims to be transferred between two parties.
-   JWT is commonly used for authentication and authorization purposes in web applications.
-   JWTs consist of three parts, separated by dots: the header, the payload, and the signature. 
-   


In NextAuth, once the user is successfully authenticated, the authorize function returns the user object. This user object can be accessed in your application via the session.user property, which is automatically set by NextAuth.

### Protected routes
### Role-Based Authentication

### middleware
- It is a way to run logic before accessing any page
- You can use a Next.js Middleware with NextAuth.js to protect your site.
- https://next-auth.js.org/configuration/nextjs#middleware

### providers
- Email and Password
- Email
- Active Directory
- Google


### Persist logged in user


https://www.youtube.com/watch?v=fYObrr3jf0w

https://www.youtube.com/@SakuraDev


Create an endpoint
/api/auth/signup


Create and send JWT


Create User Account
1. Validate user input
2. Validate user doesnt laready exist
3. Confirm Password match
4. Hash password
5. Save user
6. Create JWT
7. Send JWT to client

 ####  Hash password
 - https://www.npmjs.com/package/bcrypt








STANDARDS
Building Blocks of a Web Application
There are a few things you need to consider when building modern applications. Such as:

User Interface - how users will consume and interact with your application.
Routing - how users navigate between different parts of your application.
Data Fetching - where your data lives and how to get it.
Rendering - when and where you render static or dynamic content.
Integrations - what third-party services you use (CMS, auth, payments, etc) and how you connect to them.
Infrastructure - where you deploy, store, and run your application code (Serverless, CDN, Edge, etc).
Performance - how to optimize your application for end-users.
Scalability - how your application adapts as your team, data, and traffic grow.
Developer Experience - your team’s experience building and maintaining your application.


Settings

 Bracket Pair Colorization: Enabled






https://fkhadra.github.io/react-toastify/introduction
npm install --save react-toastify

hydration

## Deployment
Amazon EC2
RDS

npm run build
npm run start

latency

optional chaining operator
The ?. is called the optional chaining operator

The expression {data?.user ? a : b} in Next.js is using optional chaining and conditional (ternary) operator. It can be broken down into two parts:

The ?. is called the optional chaining operator. It is used to access nested properties of an object without throwing an error if the property does not exist or is null or undefined

### react-geocode
### react-map-gl
### react-date-range
https://absagroup.udemy.com/course/nextjs-dev-to-deployment/learn/lecture/26055700?start=135#overview

https://www.youtube.com/watch?v=6aP9nyTcd44

React suspence boundary



Trending - Clicks count

Infinite scrolling

Activate registration via a valid email address
Forgot and Reset password
Providers - Google,Credentials,Email,LinkedIn,Twitter