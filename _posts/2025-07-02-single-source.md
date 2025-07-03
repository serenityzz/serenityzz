---
title: "Single-sourcing"
date: 2025-06-18
tag: technical writing
---
📑   
Single-sourcing refers to the practice of creating pieces of content once and reuse them in different outputs or formats. It is commonly used in technical writing where you create content in a central place and use them in various formats such as online helps, PDFs, and printed materials. It reduces redundancy, enhances consistency, and makes content update easier to manage.   
## Use case examples<br>   
When a lot of content is shared, it can be more efficient to single source your content. <br>

- **Example 1**: Product A and Product B follow the same safety guidelines. You create a single safety guide topic and use it in both products' manauls.
- **Example 2**: You write an introcution for a new product. The docs team includes the product introduction in the user manual and the marketing team uses the same introduction in the product brochures. 

## Benefits of using single-sourcing    
Single-sourcing has the following benefits: <br>

- **Efficiency**. For the shared content, you only need to create it once and then you can reuse it often. This eliminates content duplication, saves time and improves efficiency. <br>
- **Consistency**. When there's a need to update the content, you only need to make the update in a single place and the update is reflected in all places where the content is used. This ensures content consistency across outputs and channels.<br>
- **Scalbility**. When information needs expand, single-sourcing allows easy scaling. For instance, if your product manual used to be published in PDFs only and now you also need to make it available online, with single-sourcing, you can use the same set of content to generate the HTML output.<br>

## Use single-sourcing in Flare
In previous jobs I used the Flare authoring tool. It supports single-sourcing, content reuse, conditonal content, and various outputs. In this section, I will talk about how to single-source content in Flare.<br> 
Flare supports single-sourcing at the paragraph, topic, and output levels.
In Flare you can use the snippets or sinlge project but different outputs to single source your content. <br>
### Snippets
Use snippets to create small, reusable chunks of resuable, such as paragraphs, tables, and images. When using snippets, the formating of the content is preserved. 
For example, if commands A and B share the same set of parameters, you can create a snippet containing a table that describes those parameters. Then in each topic that exaplains the two commands, you can insert the snippet.   
### Single project, different outputs
When large volumes of content can be shared, you can set up one Flare project and generate various outputs. Typical use cases of this are: <br>
- On-premises and SaaS versions of the same product. 
- A same help guide published online and in PDFs. <br>

To use a single Flare project to generate various outputs, do the following:<br>
1. Create a Flare poject and create all the topics.
2. Set up a TOC for each output.
3. Set up a target for each ouput.
4. 
