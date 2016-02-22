CREATED BY MAXIM TAM; 9/17/2015
# Automated Comic Retriever 
Comics.sh is a shell script that gathers the weekly/daily comic strips into one local folder.
Run the comics.sh to generate today's comics and use comics.html to view.
Comics.sh replaces each old strip so no old comic strip is kept.
# Run removeComics.sh to remove all generated files.
```
$ sh comics.sh
$ sh removeComics.sh
```
# To automate this for everyday retrieval using crontab on UNIX systems, do the following
1. `cd` until you reach the directory of comics.sh 
2. `pwd` and copy the output
3. `crontab -e` to enter crontab vim editor
4. press `i` to enter insert mode
5. paste `00 12 * * * <pwd output>/comics.sh` and substitute `<pwd output>` with what you copied in step 2 
6. press `esc` and `shift zz` to exit and save
