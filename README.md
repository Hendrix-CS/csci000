# Academic CSCI Course Page with Jekyll

This is the generic template for making a Computer Science course page at [Hendrix College](http://hendrix.edu). This uses [Jekyll](https://jekyllrb.com/) and [GitHub Pages](https://pages.github.com/) for deployment to the web.

Do you have improvements you would like to add? Pull Requests are welcome! Please add any errors, questions, or accessibility issues to the Issues section above.

## Examples

Links to all of the Hendrix CSCI courses using this template can be found at [hendrix-cs.github.io](https://hendrix-cs.github.io/).

## Deployment

There are just a few steps to creating a new course website from this repository.

* Determine the subdirectory you will use for this course. For example, our [CSCI 150 - Foundations of Computer Science](http://hendrix-cs.github.io/csci150) course uses `csci150`.

* Use this repository as the [template](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-repository-from-a-template) for making your new repository, named exactly with your chosen subdirectory name. Your repository can be public or private.

* Edit the `_config.yml` file on line 27, changing the `baseurl` to be your chosen subdirectory, e.g. `/csci150`.

* [Configure the repository](https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site) so that is will show up as a GitHub pages website. 

Hooray! Your course website should be visible at `https://<username>.github.io/<subdir>`.

## Content

Once your course repository is created and visible on the web, it is time to update the content.

### Background Image

The easiest way to set the jumbotron image is to copy a new image into the `assets/images` directory, and name it `jumbo-background.jpg`. Larger images are better and will be less pixelated on large screens.

For a different type of image or to have it named something else, you will need to change the filename in the `.jumbotron` class definitions in the `assets/css/main.css` file so that the src attribute shows your file.

### Description, Course Number, Title, and Semester

The `_config.yml` file contains a number of elements that can be edited to customize the course for your content.

First, replace the current `description` with the catalog copy of your course description. *Be sure it is indented to follow the YAML formatting.*

Next, change the course `number` be a human-readable version of the catalog numbering for the course, e.g. `CSCI 150`, and the `semester` to be a human-readable indicator of the semester, e.g `Fall 2019`. These will appear on the webpage in the upper-left portion of the navigation bar.

Finally, the `title` for the course should be edited to match the catalog name, e.g. `Foundations of Computer Science`.

### Navigation Bar

The `navigation` denotes the links in the top-right of the header on each page. Simple links have a `page` and `url` field, while grouping of links are denoted with a `title` field and a `subfolderitems` list of simple links.

### Instructors and Offerings

The next section of `_config.yml` defines the `instructors` for the course. An instructor has an `id`,`name`,`email` address,`web` link ,`phone` number, and `officehours` link. This information is displayed either on or near the jumbotron in the main page header.

Now, `offerings` are created, which are given a `name`, and list the room `loc`, the `time` of the offering, and the `instructor` for that offering using their `id` from above.

If there is only one offering, we recommend updating the `index.md` document to use the `course-single.md` layout instead of `course-multi.md`. It looks better.

### Resources

Resources provided to the students, such as links to software or textbooks, are listed next in the `resources` list. Each resource
has a `name`, an `image` used for easy visual reference, and a
`url` for linking to the resource. These can be displayed in a row, with a maximum of four per row, using
the template found in `_includes\resources.html`.

Additional resources in different categories can be created following the same structure, as shown with the `extra-resources` section being displayed on the `index.md` page with the Optional Resources heading.

### Labs, Homework, and Projects

Student assignments such as labs, homeworks, and projects should use the `work.html` layout. It is helpful to organize the labs, homeworks, and projects into their own directories.

The `sample-lab.md` and `sample-project.md` files are good examples of how to use markdown to write an assignment. The frontmatter at the beginning of the page is processed by the layout to display the title and number at the top of the webpage.

    ---
    layout: work
    type: Lab
    num: 4
    worktitle: Guess My Number
    ---

This can be edited for your specific assignment, and augmented to include any information you want as liquid variables within your assignment, such as the due dates in the sample project page.

We have included four [alert](https://getbootstrap.com/docs/4.0/components/alerts/) contexts to help highlight key portions of the assignments. They can be for `warning`, `tip`, `note`, or `important` sections, with their source found in the `_includes` folder, and are included using the following syntax

    {% include important.html content="Make sure your locations are chosen so that
    the face is always completely visible on the screen." %}

To make any images on your page [responsive](https://getbootstrap.com/docs/5.0/content/images/) for different browser sizes, you can add `{: .img-fluid }` after the image link.

## Customization and Style

This template is set up for Hendrix College courses, and follows the [Style Guide](https://www.hendrix.edu/WorkArea/DownloadAsset.aspx?id=86641) for our college. This section shows how to edit this for different institutions or styles.

### Colors

We use Hendrix Orange `#f5822a` as the main color theme in the header, footer, and links. This is defined, along with a few other colors, as a variable at the top of the `assets/css/main.css` file.

### Fonts

Hendrix uses the [Merriweather Sans](https://fonts.google.com/specimen/Merriweather+Sans) font on webpages. Other fonts can be [swapped out](https://stackoverflow.com/questions/14676613/how-to-import-google-web-font-in-css-file) for your particular instutituional style by changing the `@import` and `font-family` lines.
