## pixabay
Python 3 Pixabay's API wrapper.

### Install from PyPi
`pip install python-pixabay`

### Synopsis

```python
from pixabay import Image, Video

API_KEY = 'my_pixabay_api_key'

# image operations
image = Image(API_KEY)

# default image search
image.search()

# custom image search
ims = image.search(q='cats dogs',
             lang='es',
             image_type='photo',
             orientation='horizontal',
             category='animals',
             safesearch='true',
             order='latest',
             page=2,
             per_page=3)

print(ims)

# video operations
video = Video(API_KEY)

# default video search
video.search()

# custom video search
vis = video.search(q='cats', lang='fr',
                       video_type='animation',
                       category='animals',
                       page=1,
                       per_page=4)

print(vis)
```

### Usage

I wrote a few _how to_ articles in the [project wiki](https://github.com/donnmyth/pixabay/wiki). Feel free to add more examples or scenarios to the wiki.

### Running the tests

*   Make sure you've assigned the `PIXABAY_API_KEY` environment variable with your
registered Pixabay's api key.

*   Run the following command `pytest` in the project directory.

### Maintainer and Contributors

*   This software is authored and maintained by [donnmyth](https://github.com/donnmyth).

*   For contributors that contributed to this development of this module, see the
CONTRIBUTORS file.

### See Also
*   [Pixabay's API Documentation](https://pixabay.com/api/docs)

### License

This module is licensed under the MIT license. See LICENSE file for more details.
