# Berkeley CDSS Discovery Handbook

## What is this guide and who is it for?

The information in the guide is primarily intended for instructors who either currently are or will be teaching a course in the UC Berkeley Data Science Education Program: either a connector course, a data-enabled course, or a course featuring a data science module. However, anyone else who wants to learn more about the program, the courses, and the technology is encouraged to look through the guide.

## Modify This Content

Fork this repository into your own account by clicking on the `Fork` button and then `Create fork`.

Make changes in branches on your own fork, then make pull requests on this repo. Following feedback, discussion, alterations, etc., authorized staff will merge the PRs.

## Preview Changes

You can preview your changes on your own device before submitting a PR. This may catch obvious formatting issues.

1. Install a Conda distribution, such as [Miniforge](https://conda-forge.org/miniforge).
2. Install software using conda/mamba. We have provided an `environment.yml` to make this step simpler. Run the commands below to install all dependencies in a separate environment, and then activate it. This keeps your website development separate from any other projects you're working on.
```bash
# You can replace `mamba` with `conda`.
mamba env create -f environment.yml

# Now you can activate the environment.
# You can use `mamba activate` or `conda activate`, but these require that you
# have run `mamba init` or `conda init`, which modifies your shell.
mamba activate discovery-handbook

# Alternatively, you can activate without the `init` step mentioned above.
source activate discovery-handbook
```

Activate this environment whenever you start a new terminal to work on this website. Otherwise your terminal may report that it cannot find myst or its dependencies.

3. Run `myst init` in the working directory. When prompted, let the command run `myst start` for you to generate a preview. myst will display a localhost URL where the site preview is running, such as http://localhost:3000. Open this URL in your browser.

You can also run `myst build` to create static HTML (in the `_build` directory) without automatically displaying it.

Note: Do not commit the files in `_build` to the repository.
