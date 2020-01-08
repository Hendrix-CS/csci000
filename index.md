---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: course-multi
resources:
  - name: Python 3
    image: assets/images/pythonlogo.png
    url: http://python.org
  - name: Azure Notebooks
    image: assets/images/azure.png
    url: https://notebooks.azure.com/
  - name: Pycharm
    image: assets/images/pycharmlogo.png
    url: https://www.jetbrains.com/pycharm/
extra-resources:
  - name: "How to Think Like a Computer Scientist: Interactive Edition"
    image: assets/images/runestone_logo.png
    url: https://runestone.academy/runestone/books/published/thinkcspy/index.html
  - name: Python Tutor
    image: assets/images/python_tutor.png
    url: http://pythontutor.com/
  - name: CodingBat Python
    image: assets/images/codingbat.jpg
    url: https://codingbat.com/python
  - name: CheckiO Python Practice
    image: assets/images/checkio_logo_small.png
    url: https://py.checkio.org/
---

# <a name="description">Overview</a>

{{ site.description }}

## <a name="goals">Learning Goals</a>

Upon completing this course, our goal is for you to be able to:

* Build computer programs to:
  * Effectively solve realistic problems.
  * Organize, analyze, and summarize realistic data sets.
* Read, understand, and explain a computer program.
* Understand and explain computation through:
  * Thinking logically and precisely.
  * Making and testing hypotheses.
* Use modular components to decompose problems and assemble solutions.
* Create abstract, generalized models from specific, complex examples.

## <a name="resources">Resources</a>

<div class="row">
{% for res in page.resources %}
<div class="col-md-{{ 12 | divided_by: page.resources.size }}"
     style="text-align: center">
<img src="{{site.baseurl}}/{{ res.image }}" height="100" border="1">
<p>
<a href="{{ res.url }}">{{ res.name }}</a><br>
</p>
</div>
{% endfor %}
</div>

## <a name="additional-resources">Optional Resources</a>

<div class="row">
{% for res in page.extra-resources %}
<div class="col-md-{{ 12 | divided_by: page.extra-resources.size }}"
     style="text-align: center">
<img src="{{site.baseurl}}/{{ res.image }}" height="100" border="1">
<p>
<a href="{{ res.url }}">{{ res.name }}</a><br>
</p>
</div>
{% endfor %}
</div>

## Laptop Policy

Please **do not bring laptops to lecture**. This may seem strange in a computer science class. But lab is the place where you will get plenty of experience working on the computer; lecture is a time for thinking and learning without the distraction of a computer.

Exceptions may be made on a case-by-case basis if you can prove to me that you really do benefit from using your laptop to take notes.

<hr>

# <a name="inclasscode">In-Class Code</a>

When we write code together in class, it will be posted here!

| Date | Topic | 8am | 11am |
|:-:|-||-||-||
| F 30 Aug | Intro to Python | [8am](https://pythonintro-yorgey.notebooks.azure.com/j/notebooks/PythonIntro.ipynb) | [11am](https://generalnotes-goadrich.notebooks.azure.com/j/notebooks/firstnotebook.ipynb) |
| W 4 Sep | More Math and Functions | [8am](https://boxmath-yorgey.notebooks.azure.com/j/notebooks/BoxMath.ipynb) | [11am](https://generalnotes-goadrich.notebooks.azure.com/j/notebooks/Functions.ipynb) |
| F 6 Sep | Strings and Booleans | [8am](https://booleans-yorgey.notebooks.azure.com/j/notebooks/Strings%20and%20Booleans.ipynb) | [11am](https://generalnotes-goadrich.notebooks.azure.com/j/notebooks/Booleans.ipynb) |
| M 9 Sep | Conditionals | [8am](https://booleans-yorgey.notebooks.azure.com/j/notebooks/Conditionals.ipynb) | [11am](https://generalnotes-goadrich.notebooks.azure.com/j/notebooks/Strings%20and%20Conditionals.ipynb) |
| M 23 Sep | PyCharm, I/O, while | [intro.py]({{site.baseurl}}/in-class/8am/intro.py), [while.py]({{site.baseurl}}/in-class/8am/while.py) | [intro.py]({{site.baseurl}}/in-class/11am/intro.py) |
| W 25 Sep | more while loops | [while.py]({{site.baseurl}}/in-class/8am/while.py), [collatz.py]({{site.baseurl}}/in-class/8am/collatz.py) | [repetition.py]({{site.baseurl}}/in-class/11am/repetition.py), [collatz.py]({{site.baseurl}}/in-class/11am/collatz.py) |
| F 27 Sep | functions | [collatz.py]({{site.baseurl}}/in-class/8am/collatz.py), [stacktrace.py]({{site.baseurl}}/in-class/8am/stacktrace.py) | [collatz2.py]({{site.baseurl}}/in-class/11am/collatz.py) |
| M 30 Sep | function abstraction | [hilow.py]({{site.baseurl}}/code/hilow.py), [hilow_functions.py]({{site.baseurl}}/code/hilow_functions.py) | [hilow.py]({{site.baseurl}}/in-class/11am/hilow.py), [hilow_functions.py]({{site.baseurl}}/in-class/11am/hilow_functions.py)  |
| W 2 Oct | strings | [8am](https://pythonintro-yorgey.notebooks.azure.com/j/notebooks/Strings.ipynb) | [11am](https://generalnotes-goadrich.notebooks.azure.com/j/notebooks/Strings.ipynb)|
| F 4 Oct | String and loop practice | [8am](https://pythonintro-yorgey.notebooks.azure.com/j/notebooks/Strings.ipynb) | [morewhile.py]({{site.baseurl}}/in-class/11am/morewhile.py)|
| M 7 Oct | Lists | [8am](https://pythonintro-yorgey.notebooks.azure.com/j/notebooks/Lists.ipynb) | [morewhile2.py]({{site.baseurl}}/in-class/11am/morewhile2.py) |
| W 9 Oct | More lists | [8am](https://pythonintro-yorgey.notebooks.azure.com/j/notebooks/Lists.ipynb) | [listpractice.py]({{site.baseurl}}/in-class/11am/listpractice.py) |
| F 11 Oct | List practice | [8am](https://pythonintro-yorgey.notebooks.azure.com/j/notebooks/Lists.ipynb) | [fridaypractice.py]({{site.baseurl}}/in-class/11am/fridaypractice.py)|
| M 21 Oct | For loops | [For Loops.ipynb](https://pythonintro-yorgey.notebooks.azure.com/j/notebooks/For%20Loops.ipynb) | [ForLoops.ipynb](https://generalnotes-goadrich.notebooks.azure.com/j/notebooks/ForLoops.ipynb)|
| W 23 Oct | For loops with `range` | [For Loops.ipynb](https://pythonintro-yorgey.notebooks.azure.com/j/notebooks/For%20Loops.ipynb) |
| F 25 Oct | Tracing and the Heap | [References](https://pythonintro-yorgey.notebooks.azure.com/j/notebooks/References.ipynb) | [More Tracing](https://generalnotes-goadrich.notebooks.azure.com/j/notebooks/MoreTracing.ipynb) |
| M 28 Oct | Dictionaries | [Dictionaries](https://pythonintro-yorgey.notebooks.azure.com/j/notebooks/Dictionaries.ipynb) | [Dictionaries](https://generalnotes-goadrich.notebooks.azure.com/j/notebooks/Dictionaries.ipynb) |
| W 30 Oct | File Input Output | [Files](https://pythonintro-yorgey.notebooks.azure.com/j/notebooks/Files.ipynb) | [File I/O](https://generalnotes-goadrich.notebooks.azure.com/j/notebooks/FileInputOutput.ipynb) |
| F 1 Nov | Dictionary/tracing practice | [Dictionaries](https://pythonintro-yorgey.notebooks.azure.com/j/notebooks/Dictionaries.ipynb) | |
| M 4 Nov | Classes and objects | [Birthday Cake.ipynb](https://pythonintro-yorgey.notebooks.azure.com/j/notebooks/Birthday%20Cake.ipynb) | [Objects.ipynb](https://generalnotes-goadrich.notebooks.azure.com/j/notebooks/Objects.ipynb) |
| W 6 Nov | More Classes | | [MakingCake.ipynb](https://generalnotes-goadrich.notebooks.azure.com/j/notebooks/MakingCake.ipynb) |
| F 8 Nov | Designing classes | [traffic.py]({{site.baseurl}}/in-class/8am/traffic.py) | |
| M 11 Nov | Extended example | | |
| W 13 Nov | Extended example | | [Card, Hand, Deck, Player]({{site.baseurl}}/in-class/11am/CardStuff.py)|
| F 15 Nov | Extended example | [Elevator]({{site.baseurl}}/in-class/8am/Elevator.py), [Person]({{site.baseurl}}/in-class/8am/Person.py), [Hotel]({{site.baseurl}}/in-class/8am/Hotel.py), [Main]({{site.baseurl}}/in-class/8am/Main.py) | |
| MW 2-4 Dec | Queues | | |
| F 6 Dec | ? | [A different problem](https://open.kattis.com/problems/different), [Cold-puter Science](https://open.kattis.com/problems/cold), [Baby Bites](https://open.kattis.com/problems/babybites), [Saving Princess Peach](https://open.kattis.com/problems/princesspeach), [Babelfish](https://open.kattis.com/problems/babelfish) | [Graphics.py Demo Day]({{site.baseurl}}/in-class/11am/demoday.py) |

<hr>

# Coursework

Each student has **four late days** to spend throughout the semester as they wish.
Simply inform the instructor any time *prior* to the due date for an assignment
that you wish to use a late day; you may then turn in the assignment up to 24
hours late. Multiple late days may be used on the same assignment. There are no
partial late days; turning in an assignment 2 hours late or 20 hours late will
both use 1 late day. Note that late days are intended to cover both normal
circumstances (you simply want more time to work on the assignment) and
exceptional circumstances (you get sick, travel for a game or family
obligation, *etc.*). After you have used up your late days, late assignments
will receive at most half credit.

## <a name="hwqz">Homework and Quizzes</a>: 140 points

| #  | Name | Assigned | Due
|:-:|-||:-:|:-:|
|0 | [Info Sheet](https://docs.google.com/forms/d/e/1FAIpQLSdtxgmw2tL6IzzK0qq3Fw2h2FTFmGHoTRs8p6wTfTToUn7pZg/viewform?usp=sf_link) | W Aug 28 | F Aug 30 |
|1 | [Minecraft by hand]({{site.baseurl}}/homework/minecraft.html) | F Aug 30 | W Sep 4 |
|2 | [Boolean practice]({{site.baseurl}}/homework/booleans.pdf) | F Sep 6 | W Sep 11 |
|3 | [Tracing & conditional practice]({{site.baseurl}}/homework/tracing-conditional-practice.pdf) | F Sep 13 | W Sep 18 |
| |Homework Checkin 1 | M Sep 23 | F Oct 4 |
|4 | [Function and loop practice]({{site.baseurl}}/homework/function-reading.pdf) | F Sep 27 | W Oct 2 |
|5 | [Strands of DNA]({{site.baseurl}}/homework/dna-strings.html) | F Oct 4 | W Oct 9 |
|6 | [For loop reading]({{site.baseurl}}/homework/for-reading.pdf) | F Oct 25 | W Oct 30 |
|7 | [Heap/dictionary reading]({{site.baseurl}}/homework/heap-dict-reading.pdf) | F Nov 1 | W Nov 6 |
|8 | [Class design practice]({{site.baseurl}}/homework/class-design.pdf) | F Nov 8 | W Nov 13 |
|9 | [Class reading]({{site.baseurl}}/homework/class-reading.pdf) | F Nov 15 | W Nov 20 |

There will often be short homework assignments to be completed over the weekend, assigned on Friday and due Wednesday, sometimes with a corresponding quiz at the beginning of class on Wednesday.


## <a name="labs">Labs</a>: 260 points

<br/>
<div style="text-align: center; font-size: 150%; border-style: solid; border-width: 2px; width: 50%; margin: 0 auto; padding: 10px">
<a href="https://forms.gle/FDVYUUvWmg5EdFs38">Submission form</a><br>

<a href="{{site.baseurl}}/docs/lab-project-rubric.pdf">Rubric</a>
</div>
<br/>

* [Thursday lab code of conduct]({{site.baseurl}}/docs/code-of-conduct-19F-R.pdf)

| #  | Name | Assigned | Due
|:-:|-||:-:|:-:|
|1 | [Minecraft Hour of Code]({{site.baseurl}}/labs/minecraft.html) | Aug 28-29 | Sep 4-5 |
|2 | [Kepler and Newton](https://notebooks.azure.com/goadrich/projects/kepler-vs-newton) | Sep 4-5 | Sep 11-12 |
|3 | [Diagnosing Heart Disease](https://notebooks.azure.com/goadrich/projects/heart-disease-lab) | Sep 11-12 | Sep 18-19 |
|4 | [This Day in History](https://notebooks.azure.com/yorgey/projects/this-day-in-history-public) | Sep 18-19 | Sep 25-26 |
|5 | [Guess My Number]({{site.baseurl}}/labs/guess.html) | Sep 25-26 | Oct 2-3 |
|6 | [Mutation is the Word]({{site.baseurl}}/labs/doublets.html) | Oct 2-3 | Oct 9-10 |
|7 | [Todo Manager]({{site.baseurl}}/labs/todo-manager.html) | Oct 9-10 | Oct 23-24 |
|8 | [Caesar’s Secrets](https://notebooks.azure.com/goadrich/projects/caesar-s-secrets) | Oct 23-24 | Oct 30-31 |
|9 | [Sentiment Analysis](https://notebooks.azure.com/goadrich/projects/sentiment-analysis) | Oct 30-31 | Nov 6-7 |
|10| [Water Jugs]({{site.baseurl}}/labs/waterjug.html) | Nov 6-7 | Nov 13-14 |
|11| [Graphics and Animation]({{site.baseurl}}/labs/graphics.html) | Nov 13-14 | Nov 20-21 |
|12| [Enron’s Secrets]({{site.baseurl}}/labs/needles.html) | Nov 20-21 | Dec 4-5 |
|13| [On Stuckness and Debugging]({{site.baseurl}}/labs/debugging.html) | Dec 4-5 | Dec 11-12 |

Much of your experience with programming in this course will be through weekly labs. Each lab will be assigned Wednesday/Thursday in lab with time allotted to work through the materials, and will be due **by the start of the following lab**. All labs are weighted equally within the lab portion of your final grade.

On these labs, you will work with a partner on the lab assignments. Their name must be listed on any code you hand in as joint work. A partnership should only turn in a **single copy** of the assignment. If students working as partners wish to turn in a lab late, both students must use a late day.

**Lab attendance is required**. Labs take place in the **Snoddy Computer Lab**, in the Bailey Library. As you go through the exterior door of the library, turn immediately to your left and enter the Snoddy Academic Resource Center. Continue through the door at the far end of the hall into the first computer lab, and then enter the second lab at the back.

Labs should follow the [Python style guide](python_style_guide.html). You may use the automated style checker to help you catch common style errors.

#### Azure Notebook Setup

For many of the labs, we will be using Azure Notebooks. Here are specific instructions
on how to get started with these notebooks.

* First, you will need to create a free Microsoft Azure Notebook
  account. [Visit this webpage to start the process](https://notebooks.azure.com/).

* Click on the <kbd>Sign in</kbd> text in the upper-right corner of the
  page. Log in with your Hendrix email account and password.

* Next, follow the link for the specific lab for the week, and click on the green <kbd>Clone</kbd> button in the
  upper-right corner of the screen.

* This should make a copy of the project for you in your projects
  folder. Now click on <kbd>My Projects</kbd> and the name of your lab for the week.

* In your copy of the project, click on the `.ipynb`
  file in the project listing. This should open the
  notebook in the Azure Jupyter system in a separate browser tab, and
  you can start editing the file with your code. Follow the
  instructions in the file to complete this lab.

* You can save your progress using <kbd>Ctrl-S</kbd> or <kbd>Cmd-S</kbd>, and then
  return to this file any time.

* To submit your file for grading when you are finished, return to
  the lab folder listing in the <kbd>My Projects</kbd>
  tab. Select the circle to the left of the `.ipynb` file.
  Then, click on the down arrow icon in the menu, to
  the left of the trash can icon.  This will allow you to download
  the file onto your computer; then you can upload it using the
  usual turnin form.

## <a name="projects">Projects</a>: 350 points

<br/>
<div style="text-align: center; font-size: 150%; border-style: solid; border-width: 2px; width: 50%; margin: 0 auto; padding: 10px">
<a href="https://forms.gle/FDVYUUvWmg5EdFs38">Submission form</a>
</div>
<br/>

| #  | Name | Points | Assigned | Due
|:-:|-||:-:|:-:|:-:|
|1 | [Civic Assistance Q/A System](https://notebooks.azure.com/goadrich/projects/project-1) | 50  | Sep 21 | Sep 30 |
|2 | [Word Games]({{site.baseurl}}/projects/project2.html) | 100 | Oct 16 | Nov 1 |
|3 | [Final Project]({{site.baseurl}}/projects/final.html) | 200 | Nov 18 | Final Exam Day |

You will have three projects in this course, one about every five weeks. These projects will cover concepts we have discussed in class and in labs, and will be due approximately one week after they are assigned.

**You must work individually on the first two projects.** You may discuss concepts and ideas with your classmates, but the code you turn in must be your own. You will be graded not only on correctness, but also technique, documentation and evaluation of your solution. Further details on the grading standards and handin instructions for each project will be given when they are assigned.

## <a name="exams">Exams</a>: 250 points

There will be three in-class exams, the first worth 50 points and the second and
third worth 100 of your final grade. They will consist of short answer
questions along with writing and debugging code.

* Exam 1: Sep 20, covering functions, math, numerical data,
  conditionals, and binary encoding ([Practice exam]({{site.baseurl}}/docs/exam1-practice-f19.pdf))
* Exam 2: Oct 16, covering input/output, while loops, lists, and strings ([Practice exam]({{site.baseurl}}/docs/exam2-practice-f19.pdf))
* Exam 3: Nov 25, covering for loops, dictionaries, classes and objects ([Practice exam]({{site.baseurl}}/docs/exam3-practice-f19.pdf))

There is no final exam; you will complete a final project instead, as described above under Projects.

## <a name="scale">Grading Scale</a>

| Score  | Grade  |
|:-:|:-:|
| 900-1000  | A  |
| 800-899  | B  |
| 700-799  | C  |
| 600-699  | D  |
| 0-599  | F  |
