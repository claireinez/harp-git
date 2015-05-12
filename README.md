# How to Deploy a Harp App in GitHub Pages

**NOTE:** Node.js, Node Package Manager and Harp.js must be installed before proceeding. Resources are available at foot of page.

1. Create repository in GitHub / initialize with readme

2. Terminal: Clone Repository to your local machine
  * $ git clone https://github.com/**_username_**/**_repository_**

3. Go to repo directory
  * $ cd **_repository_**

4. Create new branch "gh-pages"
  * $ git checkout --orphan gh-pages

5. Remove all files in folder
  * $ git rm -rf

6. Init harp app
 * $ harp init _harp
   
  **OR**
   
   Init harp app with basic example blog template
 * $ harp init _harp --boilerplate harp-boilerplates/hb-blog

7. Compile harp app
  * $ harp compile _harp ./

8. Git add changed files
  * $ git add -A

9. Commit Git changes
  * $ git commit -a -m "_insert commit message here_"

10. Git push changes to repository
  * $ git push origin gh-pages


----------------------
Additional Resources
----------------------
* http://harpjs.com/docs/deployment/github-pages
* https://training.github.com/kit/downloads/github-git-cheat-sheet.pdf
* https://github.com/harp-boilerplates/hb-blog#controlling-your-content
* http://harpjs.com/docs/deployment/github-pages
* http://harpjs.com/docs/environment/install
