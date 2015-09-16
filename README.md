# ABACI #

This is the XNAT customization used in project ABACI.

### Installation ###

* First read the material provided by xnat: [XNAT Customization](https://wiki.xnat.org/display/XNAT/Customizing+XNAT)
* As explained above, first build your xnat version.
* Push this repo in the XNAT_HOME/projects/PROJECT directory (this will automatically add the schemas, report pages, etc.).
In order to do this correctly you should first clone the project (hg clone ...), which will create the folder abaci. Then from the XNAT_HOME/projects/PROJECT directory do:
cp -r abaci/* .
cp -r abaci/.* .
* Update and deploy your xnat (update.sh -Ddeploy=true)
* Update the database (psql -d xnat -f sql/xnat-update.sql -U "user")
* Optional: You can then move to adding the customized pipelines: [ABACI pipelines](https://bitbucket.org/nvinuesa/pipelines)


### Who do I talk to? ###

* Repo owner or admin: Nicolas Vinuesa (nicolas.vinuesa@u-bordeaux.fr)
* GIN UMR-5296, Université de Bordeaux.