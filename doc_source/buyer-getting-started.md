# Getting started<a name="buyer-getting-started"></a>

The following topics outline the process of getting started with software products as an AWS Marketplace buyer\.

**Topics**
+ [Step 1: Choose your software ](#step-1-choose-your-software)
+ [Step 2: Select your software configuration](#step-2-configure-your-software)
+ [Step 3: Launch your software on Amazon EC2](#step-3-launch-your-software-on-amazon-elastic-compute-cloud-amazon-ec2)
+ [Step 4: Manage your software](#step-4-manage-your-software)
+ [Step 5: Terminate your instance](#step-5-terminate-your-instance)
+ [For more information](#where-to-go-next)
+ [Buying products](buyer-subscribing-to-products.md)
+ [Launching software](buyer-launching-software.md)
+ [Software and services on AWS Marketplace](buyer-software-and-services.md)

For information about getting started with data products, see [Subscribing to data products on AWS Data Exchange](https://docs.aws.amazon.com/data-exchange/latest/userguide/subscribe-to-data-sets.html) in the *AWS Data Exchange User Guide*\.

The following tutorial describes the complete process of getting started with AWS Marketplace, using an Amazon Machine Image \(AMI\) product as an example\.

## Step 1: Choose your software <a name="step-1-choose-your-software"></a>

 AWS Marketplace includes the following categories of software: 
+ Infrastructure software
+ Developer tools 
+ Business software
+ Machine learning
+ IoT 
+ Professional services
+ Desktop Applications 
+ Data products

For more information, see [Product categories](buyer-product-categories.md)\.

Each major software category contains more specific subcategories\. For example, the Infrastructure software category contains subcategories such as Application Development, Databases & Caching, and Operating Systems\. Software is available as one of seven different product types, including Amazon Machine Images \(AMIs\) and software as a service \(SaaS\)\. For information about the different software types, see [Product types](buyer-product-types.md)\. 

 To aid you in choosing the software you need, AWS Marketplace provides the following information: 
+  Seller details 
+  Software version 
+  Type of software \(AMI or SaaS\), and information about the AMI if applicable 
+  Buyer rating 
+  Price 
+  Product information 

### To choose your software<a name="to-choose-your-software"></a>

1. Navigate to the [AWS Marketplace website](https://aws.amazon.com/marketplace)\. 
**Note**  
You can shop, subscribe, and launch new instances from either the public AWS Marketplace website, at [ https://aws\.amazon\.com/marketplace](https://aws.amazon.com/marketplace), or through the AWS Marketplace in the AWS console, at [ https://console\.aws\.amazon\.com/marketplace/home\#/subscriptions](https://console.aws.amazon.com/marketplace/home#/subscriptions)\.   
You can shop on the website without being signed in to your AWS account, but you must sign in to subscribe or launch products\. You must be signed in to your account to view the AWS Marketplace console\.   
The experiences across the two sites are similar\. This procedure uses the AWS Marketplace website but notes any major differences when using the console\.

1. The **Shop All Categories** pane contains the list of categories you can choose from\. You can also choose software featured in the middle pane\. For this tutorial, in the **Shop All Categories** pane, choose **Content Management**\. 

1.  From the **Content Management** list, choose **WordPress Certified by Bitnami and Automattic**\. 

1.  On the product details page, review the product information\. The product details page includes additional information such as: 
   +  Buyer rating 
   +  Support offering 
   +  Highlights 
   +  Detailed product description 
   +  Pricing details for instance types in each AWS Region \(for AMIs\) 
   +  Additional resources to help you get started 

1. Choose **Continue to Subscribe**\.

1. If you aren't already signed in, you are directed to sign in to AWS Marketplace\. If you already have an AWS account, you can use that account to sign in\. If you don't already have an AWS account, use the following steps to create one:

   1.  From the **Sign In or Create an Account** page, choose **Create a New Account**\. 

   1.  Follow the on\-screen instructions\. As part of the sign\-in procedure, you will receive a phone call and you must enter a PIN using your phone keypad\.
**Note**  
 When you create an account, AWS automatically signs up the account for all AWS services\. You are charged only for the services you use\. 

1. Read the Bitnami offer terms, then choose **Accept Terms** to agree to the subscription offer\.

1. It may take a moment for the subscription action to complete\. When it does, you receive an email message about the subscription terms, and then you're able to continue\. Choose **Continue to Configuration** to configure and launch your software\.

Subscribing to a product means that you have accepted the terms of the product\. If the product has a monthly fee, then upon subscription you will be charged the fee, which will be prorated based on the time remaining in the month\. No other charges will be assessed until you launch an Amazon Elastic Compute Cloud \(Amazon EC2\) instance with the AMI you chose\.

**Note**  
As a subscriber to a product, your account will receive email messages when a new version of the software you're subscribed to is published\.

## Step 2: Select your software configuration<a name="step-2-configure-your-software"></a>

Because we chose software as an AMI, your next step is to configure the software, including selecting the delivery method, version, and AWS Region in which you want to use the software\.

### To configure your software<a name="to-configure-software"></a>

1. On the **Configure this software** page, select **64\-bit \(x86\) Amazon Machine Image \(AMI\)** for the **Delivery Method**\.

1. Choose the latest version available for **Software Version**\.

1. Choose the **Region** you want to launch the product in, for example, **US East \(N\. Virginia\)**\.
**Note**  
As you make changes to your configuration, you might notice that the **Ami Id** at the bottom of the screen updates\. The AMI ID has the form *ami\-<identifier>*, for example, *ami\-123example456*\. Each version of each product in each Region has a different AMI\. This AMI ID allows you to specify the correct AMI to use when launching the product\. The **Ami Alias** is a similar ID that is easier to use in automation\.   
For more information about the AMI alias, see [Using AMI aliases](buyer-ami-aliases.md)\.

1. Select **Continue to Launch**\.

## Step 3: Launch your software on Amazon EC2<a name="step-3-launch-your-software-on-amazon-elastic-compute-cloud-amazon-ec2"></a>

Before you launch your Amazon EC2 instance, you need to decide if you want to launch with 1\-Click launch or if you want to launch using the Amazon EC2 Console\. 1\-Click launch helps you launch quickly with recommended default options such as security groups and instance types\. With 1\-Click launch, you can also see your estimated monthly bill\. If you prefer more options, such as launching in an Amazon Virtual Private Cloud \(Amazon VPC\) or using Spot Instances, then you should launch using the Amazon EC2 Console\. The following procedures walk you through subscribing to the product and launching an EC2 instance using either 1\-Click launch or the Amazon EC2 Console\. 

### To launch on Amazon EC2 using 1\-Click launch<a name="to-launch-on-amazon-ec2-using-1-click-launch"></a>

1.  On the **Launch this software** page, choose **Launch from website** in the **Choose Action** dropdown, and review the default settings\. If you want to change any of them, do the following: 
   + In the **EC2 Instance Type** dropdown list, choose an instance type\.
   + In the **VPC Settings** and **Subnet Settings** dropdown lists, select the network settings you want to use\.
   + In the **Security Group Settings**, choose an existing security group, or choose **Create New Based On Seller Settings** to accept the default settings\. For more information about security groups, see [Amazon EC2 security groups for Linux instances](http://docs.amazonwebservices.com/AWSEC2/latest/UserGuide/using-network-security.html) in the *Amazon EC2 User Guide for Linux Instances*\. 
   + Expand **Key Pair**, and choose an existing key pair if you have one\. If you don't have a key pair, you're prompted to create one\. For more information about Amazon EC2 key pairs, see [Amazon EC2 key pairs](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-key-pairs.html)\.

1.  When you're satisfied with your settings, choose **Launch**\. 

   Your new instance is launched with the *WordPress Certified by Bitnami and Automattic* software running on it\. From here, you can view the instance details, create another instance, or view all instances of your software\.

### To launch on Amazon EC2 Using Launch with EC2 Console<a name="to-launch-on-amazon-ec2-using-launch-with-ec2-console"></a>

1.  On the **Launch on EC2** page, choose the **Launch with EC2 Console** view, and then select an AMI version from the **Select a Version** list\. 

1.  Review the **Firewall Settings**, **Installation Instructions**, and **Release Notes**, and then choose **Launch with EC2 Console**\. 

1.  In the EC2 console, launch your AMI using the Request Instance Wizard\. Follow the instructions in [Get started with Amazon EC2 Linux instances](http://docs.amazonwebservices.com/AWSEC2/latest/GettingStartedGuide/Welcome.html?r=9803) to navigate through the wizard\. 

## Step 4: Manage your software<a name="step-4-manage-your-software"></a>

 At any time, you can manage your software subscriptions in AWS Marketplace by using the **Manage Subscriptions** page of the [ AWS Marketplace console](https://console.aws.amazon.com/marketplace/home#/subscriptions)\. On the **Manage subscriptions** page, you can do the following: 
+  View your instance status by product 
+  View your current monthly charges 
+  Run a new instance 
+  View seller profiles for your instance 
+  Manage your instances 
+  Link directly to your Amazon EC2 instance so you can configure your software 

### To manage your software<a name="to-manage-your-software"></a>

1.  Navigate to the [ AWS Marketplace console](https://console.aws.amazon.com/marketplace/home#/subscriptions), and choose **Manage subscriptions**\. 

1. Use the **Manage subscriptions** page to manage your software subscriptions\. 

## Step 5: Terminate your instance<a name="step-5-terminate-your-instance"></a>

 When you've decided that you no longer need the instance, you can terminate it\. 

**Note**  
 You can't restart a terminated instance\. However, you can launch additional instances of the same AMI\. 

### To terminate an instance<a name="to-terminate-an-instance"></a>

1.  Navigate to the [ AWS Marketplace console](https://console.aws.amazon.com/marketplace/home#/subscriptions), and choose **Manage subscriptions**\. 

1.  On the **Manage subscriptions** page, choose the software subscription that you want to terminate an instance of, and select **Manage**\. 

1. On the specific subscription page, choose **View instances** from the **Actions** dropdown list\. 

1. Select the **Region** that the instance you want to terminate is in\. This opens the Amazon EC2 Console and shows the instances in that Region in a new tab\. If necessary, you can return to this tab to see the Instance ID for the instance to close\.

1.  In the Amazon EC2 Console, choose the **Instance ID** to open the **Instance details page**\. 

1. From the **Instance state** dropdown list, choose **Terminate instance**\.

1.  Choose **Terminate** when prompted for confirmation\. Termination takes a few minutes to complete\.

## For more information<a name="where-to-go-next"></a>

 For more information about product categories and types, see [Product categories](buyer-product-categories.md) and [Product types](buyer-product-types.md)\. 

 For more information about Amazon EC2, see the service documentation at [Amazon Elastic Compute Cloud Documentation](http://docs.aws.amazon.com/ec2/)\. 

 To learn more about AWS, see [https://aws\.amazon\.com/](https://aws.amazon.com/)\. 