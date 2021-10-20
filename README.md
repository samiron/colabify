# colabify

Migrating your notebook to Google Colab needs some preparations. It's not complicated but can be monotonous. Thats where this tiny notebook comes in place.

Why you might want to use Google Colab?
* Free GPU, therefore faster training time.
* Quickly collaborate with your peer.
* etc.

Assumption:
* You already have a git project that is publicly accessible.

Steps to use:
1. Open notebook-colabify.ipynb file. You should see a `Open in Colab` button.
2. Click that button to open this file in Google colab. You will see something like the screenshot below.
3. In the red section, put the required information
    - project name: essentially a folder where your code will be checked out.
    - github_repo: the https url of your git project.
    - clone_area: 
       - Google Drive: Will mount your google drive to your colab, then checkout the project at the root of your My Drive. This will persist even after across multiple sessions.
       - Colab Space: Will checkout the code under `/content/`. This is volatile, you will need to checkout the code again for a new session.
       - None: Mainly used when you just want to get the generated code and do nothing else.
4. Run the cell
5. The yellow section in the screenshot provide some debugging information.
6. The Green section is some generated code that you need to put at the top of your work notebook.

![image](https://user-images.githubusercontent.com/115828/138094224-a5617cc9-ea31-4bf1-895a-618b44254390.png)
