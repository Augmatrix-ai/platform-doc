# Use case 3

### Advanced Customer Email Understanding

From above use-case 2 you have learnt about customer email understanding on the basis of sentiment and summary, In this scenario, we're implementing a custom text classification block for understanding customer emails based on sentiment and summary. The process involves data preparation, model training, deployment, and endpoint integration.

For this process we'll use old flow which is used in use-case&#x20;

1. Get into the Create Project Page,
2. Click on options
3. Click on Duplicate
4. click on the duplicated project and click rename&#x20;

Next step adding Another addition block to the Same flow&#x20;

1. **Download Block**:\
   Download Annotation block for Data preparation
2. **Access Component Menu**:\
   Navigate to the component menu.
3. **Drag and Drop**:\
   Drag and drop blocks to the workspace.



<figure><img src=".gitbook/assets/emailflow.webp" alt=""><figcaption></figcaption></figure>

7. **Configure Inputs**:\
   1\. Use the editor menu to configure data for the input block. \
   2\.  Select dataset of Email.\


<figure><img src=".gitbook/assets/emailinput (1).webp" alt=""><figcaption></figcaption></figure>

8. **Connect Blocks**:\
   1\. Connect input block to the GPT-extractor block.\
   2\. Drag a line between one block node to another block node to make connection.
9. **Configure GPT Extraction Block:**\
   1\. Fill the Details of instruct with this code.

<pre><code><strong>Extract Transaction ID, Amount, and Translate to English from the givenRextInput.
</strong>Fill the data extracted to outputJsonFormat, map corresponding value with respect to key of json.
</code></pre>

&#x20;    2\. Fill the Details of another code block with Output JSON to extract the Information.

```
{
    "Transaction ID": "",
    "Amount": "",
    "TranslateToEnglish": ""
}
```

<figure><img src=".gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

9. **Configure Zero-Shot Classification Block:**
   1. Configure the block with different labels to understand the emails
   2. labels are likely to be payment, delivery, food menu, coupons.&#x20;

<figure><img src=".gitbook/assets/emailzero (1).webp" alt=""><figcaption></figcaption></figure>

10. **Configure Annotation Block**
    1. add Labelstudio code to fix the labels

```json
<View>
  <Text name="text" value="$text"/>
  <Choices name="topics" toName="text" choice="single">
    <Choice value="Payment"/>
    <Choice value="food menu"/>
    <Choice value="coupons"/>
    <Choice value="delivery"/>
  </Choices>
</View>
```

<figure><img src=".gitbook/assets/emailannotation.webp" alt=""><figcaption></figcaption></figure>

10. **Run All**:
    1. Click Run-All program to start the flow running sequentially.



<figure><img src=".gitbook/assets/emailoutput.webp" alt=""><figcaption></figcaption></figure>

11. **Annotating and Saving Your Data:**
    1. Once the run is complete, go to the annotation studio.
    2. Label the emails based on their content and context.
    3. Save your annotation by giving it a name and selecting the text-classification pipeline.

By following these steps, you'll effectively set up and run the email understanding workflow.
