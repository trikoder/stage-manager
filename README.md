# Stage Manager
 
Stage Manager is a tiny wrapper around the `git-new-workdir` script and it allows easy management of newly spawned Git working directories. If you're interested in its practical uses, check out Trikoder's [blog post](http://www.trikoder.net/blog/creating-dynamic-testing-environments-with-apache-and-git-91) about dynamic testing environments.
 
## Installation
 
* Download the `stage-manager` shell script and make it executable.
* Place the [git-new-workdir](https://raw.githubusercontent.com/git/git/master/contrib/workdir/git-new-workdir) shell script in the same directory where you downloaded `stage-manager`.
* Do the safety dance.
 
## Configuration
 
There are two variables that you should change:
 
* **REPO_LOC** - Location of the main repository from which `stage-manager` will create new Git working directories.
* **SPAWN_DIR** - Name of the folder where the spawned Git working directories will reside.
 
If you want to run any commands during the creation of the Git working directories, you can place them in a file named `.bootstrap`.
 
## License
 
See the [LICENSE](LICENSE.md) file for license rights and limitations (MIT).
