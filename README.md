# Description
This is a blog for BioConductor meetups designed with *rblogdown*.
(https://aurora-mareviv.github.io/talesofr/2018/02/r-blogdown-setup-in-github-2/)

To run the site on a local machine just run:

```
install.packages("blogdown")
```

For now, open the R-studio project and :
```
blogdown::serve_site()
```

At the moment, a map of available meetups can be found in the first post of the blog.
Of course the map needs to be moved in the homepage (how? depends on the theme?).

The map is a *leaflet* htmlwidget! 

Using a manually curated tsv file of Bioconductor Meetups (in data/cities.tsv) 
and the maps::world.cities dataframe we get the lat and long of the cities to 
plot them as markers on the map.

# Additional Informations
## configuration
The *config.toml* file contains all the relevant informations for blogdown page rendering.

## themes
The selected theme is *hugo-lithium*, additional themes can be found at https://themes.gohugo.io/. 
For themes installation retrieve the github url in the form *user/themename* and use the function:
```
blogdown::install_theme("user/themename")
```

## 