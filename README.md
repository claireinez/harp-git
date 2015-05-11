# How to Deploy a Harp App in GitHub Pages

1. Create repository in GitHub / initialize with readme

2. Terminal: Clone Repository to your local machine
  * $ git clone github.com/nofootnotes/harp-git

3. Go to repo directory
  * $ cd harp-git

4. Create new branch "gh-pages"
  * $ git checkout --orphan gh-pages

5. Remove all files in folder
  * $ git rm -rf

6. Init harp app with blog
 * $ harp init _harp --boilerplate harp-boilerplates/hb-blog

7. Compile harp app
  * $ harp compile _harp ./

8. Git add changed files
  * $ git add -A

9. Commit Git changes
  * $ git commit -a -m "Harp + pages + boilerplate commit"

10. Git push changes to repository
  * $ git push origin gh-pages


----------------------
Additional Resources
----------------------
http://harpjs.com/docs/deployment/github-pages
https://training.github.com/kit/downloads/github-git-cheat-sheet.pdf
https://github.com/harp-boilerplates/hb-blog#controlling-your-content
http://harpjs.com/docs/deployment/github-pages
http://harpjs.com/docs/environment/install
