# Sparkle

API for generating sparklines as PNG, JPG and GIFs.

## Usage

Use the file extension of your desired file type in the URL.
Add the values as a comma-separated list, e.g.

https://sparklines.herokuapp.com/api/v1.png?values=1,4,5,3,2,5

The following optional query string parameters are available.

parameter | default| purpose				            		   |  
----------|--------|-----------------------------------|
line_color| 4A8FED | color of line			        		   |
height    | 30     | height of image in pixels		     |
step	    | 30     | distance between steps in pixels  |

These can be included in the query string, e.g.

https://sparklines.herokuapp.com/api/v1.png?values=1,4,5,3,2,5&height=150&line_color=F3F




## Development

Requires [ImageMagick](http://www.imagemagick.org/) >= 6.4.9.

```bash
bundle
bundle exec shotgun
```

Then open [http://localhost:9393/api/v1.png?values=1,4,5,3,2,5](http://localhost:9393/api/v1.png?values=1,4,5,3,2,5).

[![Deploy](https://www.herokucdn.com/deploy/button.svg)](https://heroku.com/deploy)
