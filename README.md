# How to Deploy a Harp App in GitHub Pages

**NOTE:** Node.js, Node Package Manager and Harp.js must be installed before proceeding. Resources are available at foot of page.

1. Create repository in GitHub / initialize with readme

2. Terminal: Clone Repository to your local machine using either HTTPS (first option) or SSH (SSH must be set up first)
  * $ git clone https://github.com/[username]/[repository]
  * $ git clone git@github.com:[username]/[repository].git

3. Go to repo directory
  * $ cd **_repository_**

4. Create new branch "gh-pages"
  * $ git checkout --orphan gh-pages

5. Remove all files in folder
  * $ git rm -rf . [don't forget the dot at the end!]

6. Init standard harp app
 * $ harp init _harp
   
  **OR**
   
   Init harp app with a random example blog template
 * $ harp init _harp --boilerplate harp-boilerplates/hb-blog

7. Compile harp app
  * $ harp compile _harp ./

8. Git add changed files
  * $ git add -A

9. Commit Git changes
  * $ git commit -a -m "_insert commit message here_"

10. Git push changes to repository
  * $ git push origin gh-pages

11. Your page can be found at [username].github.io/[repository].

If problems arise, go to 'branches' in your repo and delete your gh-pages branch and start again from Step 1!

----------------------
Additional Resources
----------------------
* http://harpjs.com/docs/deployment/github-pages
* https://training.github.com/kit/downloads/github-git-cheat-sheet.pdf
* https://github.com/harp-boilerplates/hb-blog#controlling-your-content
* http://harpjs.com/docs/deployment/github-pages
* http://harpjs.com/docs/environment/install
