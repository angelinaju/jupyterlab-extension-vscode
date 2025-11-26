# JupyterLab Extension Setup

A guide for setting up a JupyterLab extension development environment using Miniconda on Windows.

## References  
- **JupyterLab Extension Documentation**  
  https://jupyterlab.readthedocs.io/en/stable/extension/extension_tutorial.html#extension-tutorial

- **Miniconda Installation for Windows**  
  https://www.anaconda.com/docs/getting-started/miniconda/install#windows-installation

---

## Setup Instructions

### 1. Create a Conda Environment  
With Miniconda installed, open the **Anaconda PowerShell Prompt** and create a new environment containing Node.js, JupyterLab, Copier, Git, and related dependencies:

```bash 
conda create -n jupyterlab-ext --override-channels --strict-channel-priority -c conda-forge -c nodefaults jupyterlab=4 nodejs=20 git copier=9 jinja2-time
```

2. If you would like to publish your work or share it, create a new GitHub repository and ```cd``` into the folder.

3. We can activate the conda environment by opening a bash terminal and running this command: (path may differ depending on miniconda installation location)

``` bash
source C:/Users/UserName/miniconda3/Scripts/activate jupyterlab-ext
```

4. Clone the official JupyterLab Extension Examples Repository.

``` bash
git clone https://github.com/jupyterlab/extension-examples.git
```

5. Navigate into the ```extension-examples``` repository, and make changes to the toolbar-button if necessary. 

6. To build the Jupyter Lab, run ```jlpm run build``` from that repository. 

7. When complete, run ```jupyter lab``` to launch JupyterLab in the web browser.
