GeoTag-X MapReview : Map Evaluation
=======================

This is a GeoTag-X Project meant for MapReview :: MapEvaluation.

This is designed to be built in the `GeoTag-X PDF Mode` ::
```bash
cd %%PATH_OF_GEOTAGX_PROJECT_TEMPLATE_DIRECTORY%%
python build.py mapreview/ --pdf # you should use the -f flag if you want to force update the template.html file
cd mapreview/
pbs update_project #This assumes you have `pbs` correctly configured as described [here]( http://daniellombrana.es/blog/2014/07/04/commandline-candy-for-pybossa.html )
```

###Note
The tasks.csv file expects PDF files in `image_url` column and their corresponding source in `image_source` column. These PDF files should be publicly hosted, and the server where they are hosted should set the following header when serving the files :
```
Access-Control-Allow-Origin "http://mozilla.github.io"
```

For more information, check out the project's full [description][long_description].


[geotagx-project-template]:https://github.com/geotagx/geotagx-project-template
[long_description]:long_description.md
