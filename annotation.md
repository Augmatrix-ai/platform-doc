# Annotation

### Enhancing Model Training with Labelled Data

During model training, datasets often require annotations to effectively train models. Augmatrix introduces the Annotation Store, a centralized hub for storing and managing annotations. Whether it's image annotation, text annotation, or any other labelled data, the Annotation Store streamlines this process.

#### Annotation Flow in Pipelines: Tailoring Annotations for Specific Tasks

The annotation process seamlessly integrates into task-based workflows or model training processes. Currently, we support the following pipelines:

* Text-classification Pipeline Annotation
* Object-detection Pipeline Annotation
* Text-Generation Pipeline Annotation

This ensures that annotations are specifically tailored to the unique requirements of each task.

#### Example: Annotating a Sample Email

In this example, we'll walk through annotating an email. Here are the steps to follow:

1. **Custom Email Understanding Flow**:
   * Incorporate the email into a custom email understanding flow.
2. **Add Annotation Block to Component Menu**:
   * Add an annotation block to the component menu.
3. **Provide Label Studio Sample Code in the Editor Menu**:
   * Include the Label Studio sample code in the editor menu:

```xml
<View>
  <Text name="text" value="$text"/>
  <Choices name="topics" toName="text" choice="single">
    <Choice value="Payment"/>
    <Choice value="Food Menu"/>
    <Choice value="Coupons"/>
    <Choice value="Delivery"/>
  </Choices>
</View>
```

4. **Connect Input Block and Annotation Block and Run Block**:
   * Connect the input block, annotation block, and run block.
5. **Open Output of Annotation Block**:
   * Open the output page of the annotation block.
6. **Label the Data with Appropriate Labels**:
   * Label the data with the appropriate labels.
7. **Save the Annotation with Respect to Text-classification Pipeline**:
   * Save the annotation with respect to the text-classification pipeline.

By following these steps, you'll effectively annotate the email data for model training.

This documentation aims to make the annotation process clear and accessible to users. If you encounter any issues or need further assistance, feel free to reach out to our support team.
