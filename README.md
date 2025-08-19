# Lesson: Packaging Python Projects
## Overall Time: 3-4 hours

**Target Audience**: Researchers and developers who are comfortable writing Python functions and scripts but have no prior experience with creating installable packages.

**Learning Objectives**:
- Explain why packaging code is beneficial for collaboration and reproducibility.
- Structure a Python project in a standard, recognizable way.
- Define project metadata required for packaging.
- Build a distributable package from source files.
- Install a package locally for testing and development.
- Write and run a simple unit test for the package's functionality.
- Upload a package to the Test Python Package Index (TestPyPI).
- Install a package from TestPyPI using pip.

## 1. Why Python Packages? (15 minutes)

**Goal**: Motivate the need for packaging.

**The Problem**: Start with a common scenario. You've written some useful Python functions for your research. How do you share them with a collaborator?
- Emailing .py files? This can lead to versioning chaos.
- Using a shared drive? It's hard to manage dependencies.
- What if your collaborator needs to use your code in their own scripts? They would have to manually manage file paths, which is fragile and not scalable.

**The Solution: Packages!**
- A package is a standardized way of distributing and installing Python code.
- Analogy: Think of a package as a self-contained kit (like IKEA furniture). It comes with all the parts (your code), instructions on how to build it (metadata), and a list of tools you'll need (dependencies).
  
**Benefits:**
- Reusability: Easily use your code across multiple projects.
- Shareability: Others can install your code with a single command.
- Dependency Management: Clearly define what other libraries your code needs to run.
- Reproducibility: Ensures everyone is using the same version of the code.

**Key Tools We'll Use:**
- **pip**: The installer. It's the tool that reads the package instructions and puts the code in the right place.
- **PyPI** (Python Package Index): The public warehouse where thousands of Python packages are stored. This is where pip looks for packages by default.
- **TestPyPI**: A separate, "practice" warehouse. We'll use it to learn how to upload our package without cluttering the real PyPI.

## 2. Create and Structure a Simple Python Project (30 minutes)

**Goal**: Set up a standard project directory.

1. Create the project root directory:
2. Create the source directory: It's best practice to put your main source code in a src directory.
3. Create the package directory: Inside src, we'll create a directory with the same name as our package. This is where our Python files will live.
4. Add an __init__.py file: This file tells Python that the directory is a package. It can be empty.
5. Write our first module: Let's create a function that TBD . Create a new file 

## 3. Add Metadata with pyproject.toml (30 minutes)

**Goal**: Describe our project so packaging tools can understand it.

1. **Create the file**: In the root directory, create pyproject.toml.
2. Add the build system info: This tells Python what tools to use to build your package. We'll use setuptools
3. Add project metadata: This is the core information about your package.






============= Section below to be DELETED ====================




















# The Carpentries Workbench Template Markdown Lesson

This lesson is a template lesson that uses [The Carpentries Workbench][workbench]. 

## Note about lesson life cycle stage
Although the `config.yaml` states the life cycle stage as pre-alpha, **the template is stable and ready to use**. The life cycle stage is preset to `"pre-alpha"` as this setting is appropriate for new lessons initialised using the template.

## Create a new repository from this template

To use this template to start a new lesson repository, 
make sure you're logged into Github.   
Visit https://github.com/carpentries/workbench-template-md/generate
and follow the instructions.
Checking the 'Include all branches' option will save some time waiting for the first website build
when your new repository is initialised.

If you have any questions, contact [@tobyhodges](https://github.com/tobyhodges)

## Configure a new lesson

Follow the steps below to
complete the initial configuration of a new lesson repository built from this template:

1. **Make sure GitHub Pages is activated:**
   navigate to _Settings_,
   select _Pages_ from the left sidebar,
   and make sure that `gh-pages` is selected as the branch to build from.
   If no `gh-pages` branch is available, check the _Actions_ tab to see if the first
   website build workflows are still running.
   If they're not running yet, you may need to manually enable them via the _Actions_ tab.
   The branch should become available when those have completed.
1. **Adjust the `config.yaml` file:**
   this file contains global parameters for your lesson site.
   Individual fields within the file are documented with comments (beginning with `#`)
   At minimum, you should adjust all the fields marked 'FIXME':
   - `title`
   - `created`
   - `keywords`
   - `life_cycle` (the default, _pre-alpha_, is the appropriate for brand new lessons)
   - `contact`
1. **Annotate the repository** with site URL and topic tags:
   navigate back to the repository landing page and
   click on the gear wheel/cog icon (similar to ⚙️) 
   at the top-right of the _About_ box.
   Check the "Use your GitHub Pages website" option,
   and [add some keywords and other annotations to describe your lesson](https://cdh.carpentries.org/the-carpentries-incubator.html#topic-tags)
   in the _Topics_ field.
   At minimum, these should include:
   - `lesson`
   - the life cycle of the lesson (e.g. `pre-alpha`)
   - the human language the lesson is written in (e.g. `deutsch`)
1. **Adjust the 
   `CITATION.cff`, `CODE_OF_CONDUCT.md`, `CONTRIBUTING.md`, and `LICENSE.md` files**
   as appropriate for your project.
   -  `CITATION.cff`:
      this file contains information that people can use to cite your lesson,
      for example if they publish their own work based on it.
      You should [update the CFF][cff-sandpaper-docs] now to include information about your lesson,
      and remember to return to it periodically, keeping it updated as your
      author list grows and other details become available or need to change.
      The [Citation File Format home page][cff-home] gives more information about the format,
      and the [`cffinit` webtool][cffinit] can be used to create new and update existing CFF files.
   -  `CODE_OF_CONDUCT.md`: 
      if you are using this template for a project outside The Carpentries,
      you should adjust this file to describe 
      who should be contacted with Code of Conduct reports,
      and how those reports will be handled.
   -  `CONTRIBUTING.md`:
      depending on the current state and maturity of your project,
      the contents of the template Contributing Guide may not be appropriate.
      You should adjust the file to help guide contributors on how best
      to get involved and make an impact on your lesson.
   -  `LICENSE.md`:
      in line with the terms of the CC-BY license,
      you should ensure that the copyright information 
      provided in the license file is accurate for your project.
1. **Update this README with 
   [relevant information about your lesson](https://carpentries.github.io/lesson-development-training/collaborating-newcomers.html#readme)**
   and delete this section.

[cff-home]: https://citation-file-format.github.io/
[cff-sandpaper-docs]:  https://carpentries.github.io/sandpaper-docs/editing.html#making-your-lesson-citable
[cffinit]: https://citation-file-format.github.io/cff-initializer-javascript/
[workbench]: https://carpentries.github.io/sandpaper-docs/
