### What is EC2 Image Builder

GUI that helps create VM's or AMIs as Amazon Calls them. It automates the process of creating iamges > when software updates are available, Image Builder can create a new image, run validations on it, all with the updates.

Additionally, these new AMIs can be shared with other AWS Accounts.

#### Difference between AMI vs VM vs EC2

For Amazon Machine Image (AMI), an image is a template used to create an Amazon Elastic Compute Cloud (EC2) instance. It contains all the information needed to start an EC2 instance, including the operating system, applications, and configuration settings.

Imagine an image as a blueprint for a house. The blueprint contains all the details about the house, such as the number of rooms, the layout, and the materials used. Similarly, an AMI contains all the details about an EC2 instance, such as the operating system, applications, and configuration settings.

An AMI is different from a VM (virtual machine) in the sense that an AMI is a template, while a VM is a running instance of an AMI. An AMI is like a blueprint, while a VM is the actual house.

An AMI is also different from an EC2 instance in the sense that an AMI is a static image, while an EC2 instance is a running instance. An AMI is like a snapshot of an EC2 instance, while an EC2 instance is a live, running machine.

### EC2 Image Builder Terms:

Image Pipeline - Defines the configuration and end-to-end process of bulding images, including the image recipe, distibution, and test settings.

Image Recipe - Image Builder creates a recipe for each image, which can be shared, version controlled, and re-used.

Build Compontents - The Software components included in the image.

### Exam Tips

1. EC2 Image builder automates process of creating and maintaining AMIs and container images.

2. 4-Step process: Select OS, Customize with software, test, and distribute to selected regions.

3. Image Pipeline: Settings and process. Image Recipe: Source image and build components. Build Components is the software included.
