# Flow

### Flow-page Overview

The Flow-page serves as a canvas where you can construct workflows by connecting pre-built blocks. Here's a breakdown of the key elements and functionalities:

### Components

<figure><img src=".gitbook/assets/workflow (2).jpg" alt=""><figcaption></figcaption></figure>

* **Workspace**: This is where you drag and drop components from the component menu. Configure inputs using the editor menu and save or start the process of the block here.
* **Component Menu**: Pre-built blocks are listed here for selection.
* **Marketplace** : Download components from marketplace to the component menu .
* **Editor Menu**: Make changes to the workspace as per your requirements.

### Crafting Your Workflow: A Step-by-Step Guide

#### The Art of Drag and Drop

Move blocks from the Component store to the workspace with ease. It's all about matching the right components, like fitting puzzle pieces together based on their data types.

#### Understanding Block Statuses

1. Block status and Error:
   1. **Configuration Errors**: Think of these as alerts that something's not quite right with your setup.

<figure><img src=".gitbook/assets/image.png" alt="" width="205"><figcaption></figcaption></figure>

2\. **Dataset-Level Errors**: These indicate issues within your data, but don't worry, not all is lost—some parts can still proceed.

<figure><img src=".gitbook/assets/image (1).png" alt="" width="205"><figcaption></figcaption></figure>

3\. **Success Indicators**: this indicates Your block is correctly configured, and your data is flowing smoothly.

<figure><img src=".gitbook/assets/image (2).png" alt="" width="205"><figcaption></figcaption></figure>

Connecting Blocks: The Right Fit\
1\. **Correct Connection**: ensure the data types align for a perfect fit.

<figure><img src=".gitbook/assets/image (3).png" alt="" width="375"><figcaption></figcaption></figure>

2\. Incorrect connection: this means you've connected but issue with data type mismatch

<figure><img src=".gitbook/assets/image (4).png" alt="" width="375"><figcaption></figcaption></figure>

Dive into Block Data

Observe the block you're able to understand the data type ,if you hover into the connection or node point you're able to see the variables.

2. Editor menu: This menu various Functionalities here all the list.

<figure><img src=".gitbook/assets/console.png" alt=""><figcaption></figcaption></figure>

1. **Save**: Preserve created components for future modification or processing
2. **Run All**: Execute all functions sequentially after configuring block properties and inputs without interruption.
3. **Run** : Run individual blocks one-by-one to perform specific functions.
4. **Undo**: Reverse the last user action in case of mistakes or changes of mind.
5. **Redo**: Repeat the last undone action, useful for correcting mistakes or reapplying changes.
6. **Lock**: Restrict block movement in the workspace by locking components; unlock to enable movement.
7. **Zoom In**: Enlarge workflow for focusing on specific details.
8. **Fit**: Adjust workflow to fit within the visible or reset to original size.
9. **Zoom Out**: Reduce the size of displayed content to see more on the screen at once.
10. **Deploy**: When ready to take use cases live, deploy seamlessly using various modes (scheduled, Web Endpoint, or Event Driven).
11. **Console**: The Console lets you see the activity logs of each block in your workflow. This helps you track what each block is doing and if there are any issues.

### Example Use Case: Customer Email Understanding

In this example, you'll understand emails and respond according to the email context using sample data and pre-built blocks.\\

1. **Upload Dataset**:\
   Upload the dataset to the default datastore provided by Augmatrix.io.

Here is the sample dataset providing for testing purpose

{% embed url="https://drive.google.com/file/d/1-YYFla8XHBaVICErVVgOirwLpMrSJTZR/view?usp=drive_link" %}
sample data
{% endembed %}

1. **Create Sample Project**:\
   Create a sample project in APPS.
2. **Enter Project**: Access the project.
3. **Open Component Store**:\
   Open the component store.
4. **Download Blocks**:\
   Download input and GPT-extractor blocks.
5. **Access Component Menu**:\
   Navigate to the component menu.
6. **Drag and Drop**:\
   Drag and drop blocks to the workspace.

<figure><img src=".gitbook/assets/emailflow.jpg" alt=""><figcaption></figcaption></figure>

1. **Configure Inputs**:\
   Use the editor menu to configure data for the input block.

<figure><img src=".gitbook/assets/emailinput.jpg" alt=""><figcaption></figcaption></figure>

1. **Connect Blocks**:\
   Connect input block to the GPT-extractor block.

<figure><img src=".gitbook/assets/emailgpt.jpg" alt=""><figcaption></figcaption></figure>

1. **Run All**:\
   Click Run-All program to start the flow running sequentially.
2. **Check Outputs**:\
   Examine the output of individual blocks.

<figure><img src=".gitbook/assets/emailoutput.jpg" alt=""><figcaption></figcaption></figure>

By following these steps, you'll effectively set up and run the email understanding workflow.

### Pan-card Extraction Use-case

In this example, we'll delve into the intricacies of the Pan Card extraction process. We'll elucidate each step of the workflow, detailing the configurations of individual blocks and the final output.

Moreover, we'll showcase how this flow can be adapted for extracting Aadhaar cards or similar documents.

<figure><img src=".gitbook/assets/flow.jpg" alt=""><figcaption><p>Sample Work-flow image</p></figcaption></figure>

1. **Input Configuration:** Begin by configuring the dataset you wish to process and execute the respective block.

<figure><img src=".gitbook/assets/paninput.jpg" alt=""><figcaption></figcaption></figure>

here, Pan-card is selected as the input to extract the data

2. **OCR (Optical Character Recognition) Block:** The OCR block extracts data from images provided by the input block. It outputs the extracted data in both JSON and text formats.

<figure><img src=".gitbook/assets/ocr.jpg" alt=""><figcaption></figcaption></figure>

3. **Rotate Block:** This block adjusts the angle of the card to ensure proper alignment for processing. It takes an image and OCR JSON as input to correct the orientation.

<figure><img src=".gitbook/assets/panrotate.jpg" alt=""><figcaption></figcaption></figure>

4. **Constant Block:** Containing fixed information of a reference image, this block serves as a benchmark for aligning input card images. It provides a standard reference for comparison

<figure><img src=".gitbook/assets/constant-input.jpg" alt=""><figcaption></figcaption></figure>

Here we've provided one sample reference image to extract

5. **OCR (Constant Block):** Similar to the OCR block, this component processes the reference image provided by the Constant Block and produces JSON and text outputs.

<figure><img src=".gitbook/assets/constant-ocr.jpg" alt=""><figcaption></figcaption></figure>

6. **Rotate Block (Constant Block):** This block, like the previous Rotate Block, corrects the orientation of the reference image based on the OCR results obtained from the Constant Block.

<figure><img src=".gitbook/assets/constantrotate.jpg" alt=""><figcaption></figcaption></figure>

7. **Alignment Block:** Utilizing the data from the Constant Block, this component aligns the information extracted from input cards with the standard reference.
8. **Annotation Block:** Primarily used for labeling data, the Annotation Block annotates the extracted information and facilitates the extraction of labeled data.

<figure><img src=".gitbook/assets/annotation.jpg" alt=""><figcaption></figcaption></figure>

9. **Output:** The final output encapsulates comprehensive information, including aligned data and labelled information, providing a cohesive overview of the extracted data.

<figure><img src=".gitbook/assets/panoutput.jpg" alt=""><figcaption></figcaption></figure>

By following, the above structured workflow and configuring each block appropriately, one can efficiently extract data from Pan Cards or similar documents. This adaptable approach can be extended to extract data from various document types, such as Aadhaar cards, with minor adjustments to the configurations.

\\

<figure><img src=".gitbook/assets/annotation.webp" alt=""><figcaption></figcaption></figure>
