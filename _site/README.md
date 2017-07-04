# mobtechlab.github.io

## Adding new research 
There are two to ways to add new research to the `/research` page. Neither way will require you to restart the website, Github Pages (our webhost) will automatically re-build the page on each commit (change) to the repository.

### Directly via Github
You can add a new Bibtex entry directly to the `research.txt` file on Github, found **[here](https://github.com/mobiletechlab/mobiletechlab.github.io/blob/master/research.txt)**. Simply add a new entry representing your paper, then commit the change.

### Locally on your computer, then push to Github
First, this approach requires you to clone this repository to your machine. If you've already done that, you can change the `research.txt` file found at the root of the project folder. After completing your modification to the file, commit and push the change back to Github.

## Adding new gallery entry
To add a new entry to the [gallery page](http://mobiletechlab.no/lab/gallery/), navigate to the */lab/gallery/index.html* file. At the top of that file, you'll find an "array" of gallery entries. The name of the array is ```gallery_images```, and each new element in the array starts with a - (dash). An example is seen below, where a new element starts with the dash (-), then the ```image:``` property and  value, then a ```subtitle:``` property and value. Both of these properties must be added for each new entry in the gallery. To add an image, simply paste the image into the */images/gallery/* folder, and commit&push the code back to github, and add the path to the value of the ```image:``` property in the entry.
```
gallery_images:
- image: /images/gallery/research.jpg
  subtitle: Subtitle of gallery entry
```

## Adding new project entry
To add a new entry to the [projects page](http://mobiletechlab.no/lab/projects/), navigate to the */lab/projects/index.html* file. At the top of that file, you'll find an "array" of project entries. The name of the array is ```project_entries```, and each new element in the array starts with a - (dash). An example is seen below, where a new element starts with the dash (-), then the ```image:``` property and  value, a ```title:``` property and value, and a ```text``` property and value . All these properties must be added for each new entry on the projects page. To add an image, simply paste the image to the */images/gallery/* folder, and commit&push the code back to github, and add the path to the value of the ```image:``` property in the entry.
```
gallery_images:
- image: /images/projects/image.jpg
  title: Title of the project
  text: Text describing the project entry
```