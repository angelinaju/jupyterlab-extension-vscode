# jupyterlab-extension-vscode

[JupyterLab Extension Documentation](https://jupyterlab.readthedocs.io/en/stable/extension/extension_tutorial.html#extension-tutorial)

[Miniconda Installation for Windows](https://www.anaconda.com/docs/getting-started/miniconda/install#windows-installation)

1. Assuming we have miniconda installed on the machine, we can install NodeJS, JupyterLab, copier, and git within the conda environment. Open the "Anaconda Powershell Prompt" and run the following command:

`conda create -n jupyterlab-ext --override-channels --strict-channel-priority -c conda-forge -c nodefaults jupyterlab=4 nodejs=20 git copier=9 jinja2-time`

2. Create a new repository if the user would like to publish to GitHub or share. Cd into this repository.

3. We can activate the conda environment by opening a bash terminal and running this command: (may differ depending on miniconda installation location)

`source C:/Users/UserName/miniconda3/Scripts/activate jupyterlab-ext`

4. Clone the repository of extension examples from JupyterLab.

`git clone https://github.com/jupyterlab/extension-examples.git`

5. Cd into the `extension-examples` repository, and make changes to the toolbar-button if necessary. 

6. To build the Jupyter Lab, run `jlpm run build` from that repository. 

7. When complete, run `jupyter lab` to launch JupyterLab in the web browser.