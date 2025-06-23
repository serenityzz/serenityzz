---
title: "Is Flare DITA?"
date: 2025-06-18
tags: technical writing, DITA
---
💻 📝<br>
During an interview for a technical writer, I mentioned that we were using MadCap Flare as the authoring and output generation tool. One interviewer asked if Flare was DITA.    
DITA and Flare share some similar concepts and features such as topic-based authoring, single-sourcing, and content reuse, but they are not the same thing. 

## DITA and Flare
**DITA** stands for Darwin Information Type Architecture, is a content management approach that features modular and reusable content.    
Flare is an authoring tool proprietary to the MadCap software company. It also features modular and reusable content.     

### Similarities between DITA and Flare
DITA and Flare share the following similarities.    
| Feature | Description | 
|:---|:---|
| **Topic-based authoring** | Both are topic-based. You write content in small, reusable chunks called topics and reuse them in multiple outputs, for online help and printed materials, or in differnt channels like user manuals and marketing brochures. |
| **Content reuse** | Reuse content for various outputs or channels. <ul><li>In DITA, use conref, keys, and profiling.</li><li>In Flare, use snippets and variables.</li></ul> |
| **Conditional content** | Condition content for multiple audiences or purposes. <ul><li>In DITA, use conref, keys, profiling, and filtering with attributes.</li><li>In Flare, use conditions at the sentence, paragraph, topic, and target levels.</li></ul> |
| **Multiple output formats** | Both support various output formats such as HTML, PDF, and so on. |

## Is Flare DITA?
Although Flare shares some core concepts with DITA, it does not mean Flare is DITA. The reasons are as follows:
- Flare is a tool that is proprietary to the MadCap company; while DITA is an open standard that is supported by multiple tools. 
- Although both are topic-based, in DITA topics must strictly follow the predefined information types:
   - **Task**. Describes how to do something via step-by-step instructions.
   - **Concept**. Describes a general idea, definition, or principle. 
   - **Reference**. Describes command syntax, programming instructions, and other reference materials. In DITA, images, video files, or other files that need to appear in a topic are inserted via a reference to them.
     
    Misuse of topic types may result in failure to process and structure the content correctly.  
    
- DITA strictly follows the XML format and uses the XML tags; Flare, also XML-based, supports HTML tags and MadCap XML tags. <br> 

In summary, Flare is inspired by and follows DITA's pricinples, but it does not create true DITA content. 
