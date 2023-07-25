# Introduction to ESP RainMaker

The Internet of Things (IoT) offers endless possibilities to change the way people live, yet the development of IoT engineering is full of challenges. With public clouds, terminal manufacturers can implement product functionality through the following solutions:

## Based on solution providers' cloud platforms

In this way, terminal manufacturers only need to design the product hardware, then connect the hardware to the cloud using provided communication module, and configure the product functions following the guidelines. This is an efficient approach since it eliminates the need for server-side and application-side development and operations and maintenance (O&M). It allows terminal manufacturers to focus on hardware design without having to consider cloud implementation. However, such solutions (e.g., device firmware and App) are generally not open source, so the product functions will be limited by provider's cloud platform which cannot be customized. Meanwhile, the user and device data also belong to the cloud platform.

## Based on cloud products

In this solution, after completing the hardware design, terminal manufacturers not only need to implement cloud functions using one or more cloud products provided by the public cloud, but also need to link the hardware with the cloud. For example, to connect to Amazon Web Services (AWS), terminal manufacturers need to use AWS products such as Amazon API Gateway, AWS IoT Core, and AWS Lambda to enable device access, remote control, data storage, user management, and other basic functions. It not only asks terminal manufacturers to flexibly use and configure cloud products with in-depth understanding and rich experience, but also requires them to consider the construction and maintenance cost for initial and later stages This poses great challenges to the company's energy and resources.

<br></br>
Compared with public clouds, private clouds are usually built for specific projects and products. Private cloud developers are given highest level of freedom in protocol design and business logic implementation. Terminal manufacturers can make products and design schemes at will, and easily integrate and empower user data. Combining the high security, scalability and reliability of public cloud with the advantages of private cloud, Espressif launched ESP RainMaker, a deeply integrated private cloud solution based on Amazon cloud. Users can deploy ESP RainMaker and build private cloud simply with an AWS account.