# Flow

### Flow-page Overview

The Flow-page serves as a canvas where you can construct workflows by connecting pre-built blocks. Here's a breakdown of the key elements and functionalities:

### Components

* **Workspace**: This is where you drag and drop components from the component menu. Configure inputs using the editor menu and save or start the process of the block here.
* **Component Menu**: Pre-built blocks are listed here for selection.
* **Component Store**: Download components to the component menu from here.
* **Editor Menu**: Make changes to the workspace as per your requirements.

#### Functionalities

* **Save**: Preserve created components for future modification or processing.
* **Run All**: Execute all functions sequentially after configuring block properties and inputs without interruption.
* **RUN**: Run individual blocks one-by-one to perform specific functions.
* **Undo**: Reverse the last user action in case of mistakes or changes of mind.
* **Redo**: Repeat the last undone action, useful for correcting mistakes or reapplying changes.
* **Lock**: Restrict block movement in the workspace by locking components; unlock to enable movement.
* **Zoom In**: Enlarge displayed content for focusing on specific details.
* **Fit**: Adjust displayed content to fit within the visible area of the screen or window.
* **Zoom Out**: Reduce the size of displayed content to see more on the screen at once.
* **DEPLOY**: When ready to take use cases live, deploy seamlessly using various modes (scheduled, Web Endpoint, or Event Driven).
* **Console**: CLI for live coding on the component level and executing live.

### Example Use Case: Customer Email Understanding

In this example, you'll understand emails and respond according to the email context using sample data and pre-built blocks.\


1. **Upload Dataset**: \
   Upload the dataset to the default datastore provided by Augmatrix.io.

Here is the sample dataset providing for testing purpose&#x20;

{% embed url="https://drive.google.com/file/d/1-YYFla8XHBaVICErVVgOirwLpMrSJTZR/view?usp=drive_link" %}
sample data
{% endembed %}

1. **Create Sample Project**:\
   &#x20;Create a sample project in APPS.
2. **Enter Project**: Access the project.
3. **Open Component Store**: \
   Open the component store.
4. **Download Blocks**: \
   Download input and GPT-extractor blocks.
5. **Access Component Menu**: \
   Navigate to the component menu.
6. **Drag and Drop**: \
   Drag and drop blocks to the workspace.
7. **Configure Inputs**:\
   &#x20;Use the editor menu to configure data for the input block.
8. **Connect Blocks**: \
   Connect input block to the GPT-extractor block.
9. **Run All**: \
   Click Run-All program to start the flow running sequentially.
10. **Check Outputs**: \
    Examine the output of individual blocks.

By following these steps, you'll effectively set up and run the email understanding workflow.
