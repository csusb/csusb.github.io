
To generate site locally, run the following.

    jekyll build

To run a local Web server to test the site, run the following.

    jekyll serve

However, it is possible to browse the files directly 
from the file system without running a Web server.
To do this, create filed _config.yml_ with something like the 
following contents.

````
safe: true  # disable plugins; matches Github Pages
exclude: [ README.md ]
url: file:///users/turner/git/test/_site/
````

Then generate the website as follows.

    jekyll build --config config.yml

Add _config.yml_ to _.gitignore_ because it is a setting local
to the developer's specific environment.

