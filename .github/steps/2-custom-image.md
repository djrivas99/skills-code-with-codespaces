<!--
   <<< Author notes: Step 2 >>>
   Start this step by acknowledging the previous step.
   Define terms and link to docs.github.com.
-->
# Step 2: Add a custom image to your codespace

To add a custom image to your codespace, you can specify the URL of the image in the `devcontainer.json` file. Here's an example:

[Link to custom image](https://th.bing.com/th/id/OIP.koEvj0q1HeFTpeVQ2-OD-AAAAA?rs=1&pid=ImgDetMain)

_Nice work! :tada: You created your first codespace and pushed code using VS Code!_

You can configure the development container for a repository so that any codespace created for that repository will give you a tailored development environment, complete with all the tools and runtimes you need to work on a specific project.

**What are development containers?** Development containers, or dev containers, are Docker containers that are specifically configured to provide a fully featured development environment. Whenever you work in a codespace, you are using a dev container on a virtual machine.

A dev container file is a JSON file that lets you customize the default image that runs your codespace, VS code settings, run custom code, forward ports and much more!

Let's add a `devcontainer.json` file and add a custom image.

## :keyboard: Activity: Add a .devcontainer.json file to customize your codespace

1. Navigating back to your **Code** tab of your repository, click the **Add file** drop-down button, and then click `Create new file`.
      .devcontainer/devcontainer.json

# modified:   .github/steps/2-custom-image.md
