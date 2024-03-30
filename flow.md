# Flow

Flow-page Overview

The Flow-page serves as a canvas where you can construct workflows by connecting pre-built Components. Here's a breakdown of the key elements and functionalities.

### Components

<figure><img src=".gitbook/assets/Untitled design (2).jpg" alt=""><figcaption></figcaption></figure>

* **Workspace**: This is where you drag and drop components from the component menu. Configure inputs using the editor menu and save or start the process of the Component here.
* **Component Menu**: Pre-built components are listed here for selection.
* **Marketplace** : Download components from marketplace to the component menu.
* **Editor Menu**: Make changes to the workspace as per your requirements.

1. **Editor menu**

<figure><img src=".gitbook/assets/console.png" alt=""><figcaption></figcaption></figure>

* **Save**: Preserve created components for future modification or processing.
* **Run** : Run individual components  one-by-one to perform specific functions.
* **Undo**: Reverse the last user action in case of mistakes or changes of mind.
* **Lock**: Restrict Component movement in the workspace by locking components; unlock to enable movement.
* **Notification**:  it contains product updates, Workflow Notifications etc.&#x20;
* **Menu:**  In this menu you can see these options.
* **Run All**: Execute all functions sequentially after configuring Component properties and inputs without interruption.
* **Zoom In**: Enlarge workflow for focusing on specific details.
* **Fit**: Adjust workflow to fit within the visible or reset to original size.
* **Zoom Out**: Reduce the size of displayed content to see more on the screen at once.
* **Deploy**: When ready to take use cases live, deploy seamlessly using various modes (scheduled, Web Endpoint, or Event Driven).
* **Redo**: Repeat the last undone action, useful for correcting mistakes or reapplying changes.
* **Console**: The Console lets you see the activity logs of each Component in your workflow. This helps you track what each Component  is doing and if there are any issues.

### Crafting Your Workflow: A Step-by-Step Guide

1. **The Art of Drag and Drop**
   * Move Components from the Component store to the workspace with ease. It's all about matching the right components, like fitting puzzle pieces together based on their data types.
2. **Understanding Component State:**

<figure><img src=".gitbook/assets/Untitled design.png" alt="" width="188"><figcaption></figcaption></figure>

* First DOT Indicates Component Status
* Second DOT Indicates RUN status

3.  There are different Colours to indicate component Issues

    * **Red** Colour Indicates **Error**&#x20;
    * **Yellow** Colour indicates **Warning**
    * **Blue** Colour Indicates **Success**&#x20;
    * **Grey**  Colour Indicates **Not Configured**&#x20;


4. **Component States:**

* &#x20;Configuration Errors: Think of these as alerts that something's not quite right with your setup.

<figure><img src=".gitbook/assets/image (3).png" alt="" width="205"><figcaption></figcaption></figure>

* Runtime Warning : These indicate issues with a few of yours data, and rest of the data is successfully processed.&#x20;

<figure><img src=".gitbook/assets/image.png" alt="" width="205"><figcaption></figcaption></figure>

*   Runtime error: These indicate, the Component ran without data and correct Configurations.

    <figure><img src=".gitbook/assets/image (4).png" alt="" width="205"><figcaption></figcaption></figure>

&#x20;

* Success Indicators: This indicates Your Component is correctly configured, and your data is  \
  flowing smoothly.

<figure><img src=".gitbook/assets/image (2) (1).png" alt="" width="205"><figcaption></figcaption></figure>

2.  **Connecting Components:** The Right Fit

    * &#x20;Correct Connection: ensure the data types align for a perfect fit.

    <figure><img src=".gitbook/assets/image (3) (1).png" alt="" width="375"><figcaption></figcaption></figure>

    * Incorrect connection: this means you've connected but issue with data type mismatch

    <figure><img src=".gitbook/assets/image (4) (1).png" alt="" width="375"><figcaption></figcaption></figure>
3. **Dive into  Component Data**
   * Observe the Component you're able to understand the data type, if you hover into the connection or node point you're able to see the variables.
