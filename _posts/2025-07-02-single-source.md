---

title: "Introduction to single-sourcing in technical writing"
date: 2025-07-03
tag: technical writing

---

📑   
This topic introduces single-sourcing in technical writing, its benefits, and how to apply it in Flare.<br>

## Overview

Single-sourcing is the practice of creating content once and reusing it in various places. It is commonly used in technical writing where you create content in a central place and use it in various formats such as online helps and PDFs. Single-sourcing reduces redundancy, enhances consistency, and simplifies content management.<br>

Here are some use case examples.<br>

- **Example 1**: Both the Product A and Product B follow the same safety guidelines, so you can create a single safety guide and reuse it in both products' manuals. 
- **Example 2**: You write an introduction for a new product and include it in the product's user guide and administration guide. 

## Benefits of single-sourcing

When a lot of content can be shared, single-sourcing provides the following benefits: <br>

- **Efficiency**. For shared content, you only need to create it once and can reuse it across various outputs. This eliminates content duplication, saves time, and improves efficiency. <br>
- **Consistency**. When there's a need to update the content, you only need to make the update in a single place and the update is reflected in all places where the content is used. This ensures content consistency across outputs and channels, helping maintain a unified user experience.<br>
- **Scalbility**. When information needs expand, single-sourcing allows easy scaling. For example, your product manual was published in PDFs and now also needs to be available online. With single-sourcing you can generate the HTML output using the existing content.

## Single-sourcing in Flare

This section provides details on how to apply single-sourcing in Flare. You can use snippets and conditional text in topics to single source your content.<br> 

### Snippets

Snippets are small chunks of reusable content, such as paragraphs, tables, and images. You use snippets when the shared content is small, usually in paragraphs and insert the snippets in various topics. When using snippets, the formating of the content is preserved.<br> 
For example, if commands A and B share the same set of parameters, you can create a snippet containing a table that describes those parameters, and then insert the snippet in each individual topic that explains the two commands.   

### Topics with conditional text

When larger pieces of content can be shared, you can single source and reuse the content at the topic level. For example, you create a topic introducing a product and then use this topic in both the user guide and administration guide. <br>
If some sentences or paragraphs in the topic require different content for different guides (such as a feature only available to admins), you can use conditional text in the relevant sentence or paragraph. <br>

In this example, to publish an admin-specific feature in the administration guide while hide it in the user guide, do the following:

1. Add a condition named **admin**.
2. Apply the **admin** condition to content only available to admins.
3. In the admin guide, configure to include content labeled with the **admin** condition. In the user guide, configure to exclude content labeled with the **admin** condition. 
