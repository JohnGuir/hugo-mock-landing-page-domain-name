# hugo-mock-landing-page-domain-name
Part III of Homework 2 - An autodeployed landing page that also employs a custom domain name. This project involves 



# Workflow Summary 
## (.github/workflows/gh-pages-deployment.yaml)

The workflow is designed to build and deploy a Hugo website to GitHub Pages whenever changes are pushed to the main branch of the repository. The first few steps set up the environment by checking out the repository, fetching the necessary submodules (which may include Hugo themes), and installing the specified version of Hugo with extended functionality.

The peaceiris/actions-hugo action is used to handle the Hugo environment setup, ensuring that the correct version of Hugo is installed and ready for use. The next step compiles the Hugo static files using the hugo command with flags for including drafts, enabling garbage collection, and minifying the output. Finally, the peaceiris/actions-gh-pages action is utilized to deploy the compiled website to the gh-pages branch of the repository, which is the branch used by GitHub Pages to serve the website. This action automates the process of creating or updating the gh-pages branch, copying the static files, and committing the changes.
