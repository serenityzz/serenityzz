---
title: "Introduction to single-sourcing in technical writing"
date: 2025-07-03
tag: technical writing
---
📑   
This topic introduces single-sourcing in technical writing, its benefits, and how to apply it in Flare.<br>
## Overview
Single-sourcing is the practice of creating content once and reusing it across various outputs and formats. It is commonly used in technical writing where you create content in a central place and use it in various formats such as online helps, PDFs, and printed materials. It reduces redundancy, enhances consistency, and simplifies content update. 
## Use case examples<br>   
When a lot of content is shared, it can be more efficient to single source the content. Here are some use case examples.<br>

- **Example 1**: Both the Product A and Product B follow the same safety guidelines, so you can create a single safety guide and reuse it in both products' manuals. 
- **Example 2**: You write an introduction for a new product. The docs team includes the product introduction in the user manual, while the marketing team uses the same introduction in the product brochures.

## Benefits of single-sourcing    
Single-sourcing provides the following benefits: <br>

- **Efficiency**. For shared content, you only need to create it once and it can be reused across various outputs. This eliminates content duplication, saves time, and improves efficiency. <br>
- **Consistency**. When there's a need to update the content, you only need to make the update in a single place and the update is reflected in all places where the content is used. This ensures consistent content across outputs and channels, helping maintain a unified user experience.<br>
- **Scalbility**. When information needs expand, single-sourcing allows easy scaling. For instance, if your product manual was published in PDFs but now needs to be available online, single-sourcing allows you to generate the HTML output using the existing content.

## Single-sourcing in Flare
This section provides details on how to apply single-sourcing in Flare.<br> 
Flare supports single-sourcing at the paragraph, topic, and output levels. <br>
### At paragraph level
Use snippets to single source small chunks of reusable content, such as paragraphs, tables, and images. When using snippets, the formating of the content is preserved. For example, if commands A and B share the same set of parameters, you can create a snippet containing a table that describes those parameters. Then you insert the snippet in each respective topic that describes the two commands.   
### At topic level
When larger pieces of content can be shared, you can single source and reuse the content at the topic level. For instance, you create a topic introducing a product and then use this topic in the product's user guide and administration guide. If some sentences or paragraphs in the topic require different content for different guides (such as a feature only available to admins), you can use conditional text in the relevant sentence or paragraph.  
### At output level
When large volumes of content (like most content in a guide) can be shared, you can set up one Flare project and generate various outputs. Typical use cases of this are: <br>
- On-premises and SaaS versions of the same product. 
- A same help guide published online and in PDFs. <br>

To use a single Flare project to generate various outputs, do the following:<br>
1. Set up a TOC for each output.
3. Set up a target for each ouput.
4. For topics that require different content for each output, you can use conditional content or snippets. For details, see [At paragraph level](#at-paragraph-level) and [At topic level](#at-topic-level).
