# Generic Hendrix CSCI Course Page

This is the generic template for making a Computer Science course page at [Hendrix College](http://hendrix.edu). This uses [Jekyll](https://jekyllrb.com/) and [GitHub Pages](https://pages.github.com/) for deployment to the web.

## Deployment

There are just a few steps to creating a new course website from this repository.

* Determine the subdirectory you will use for this course. For example, our [CSCI 150 - Foundations of Computer Science](http://hendrix-cs.github.io/csci150) course uses `csci150`.

* Create a new repository on GitHub named exactly with your subdirectory name. Use this as the [template](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template) for the new repository.

* Edit the `_config.yml` file on line 27, changing the `baseurl` to be your chosen subdirectory, e.g. `/csci150`.

* [Configure the repository](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site) so that is will show up as a GitHub pages website. It will be found at `<username>.github.io/<subdir>`.

## Customization

### Course Title, Number, and Semester

### Instructors and Offerings

### Navigation Bar

### Resources



### Background Image

The easiest way to set the jumbotron image is to copy a new image into the `assets/images` directory, and name it `jumbo-background.jpg`. If you want a different type image or to have it named something else, you will need to change line 29 in the `assets/css/main.css` file so that the src attribute shows your file.

### Colors

Change top and bottom bar color from Hendrix Orange to something else?

### Labs, Homework, and Projects

Adding in the note, warning tags. Using the due dates at the top in the frontmatter.
