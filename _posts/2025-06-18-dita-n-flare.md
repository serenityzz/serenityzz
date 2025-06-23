---
title: "Is Flare DITA?"
date: 2025-06-18
tags: technical writing, DITA
---
💻 📝<br>
During an interview for a technical writer, I mentioned that we were using MadCap Flare as the authoring and output generation tool. One interviewer asked if Flare was DITA. Another interviewr explained that MadCap Flare was not DITA. Well, I was not quite sure, so I did some researches about DITA and MadCap Flare. 

## DITA and Flare
**DITA** stands for Darwin Information Type Architecture, is a content management approach that features modular and reusable content.    
Flare is an authoring tool proprietary to the MadCap software company. It also features modular and reusable content.     
DITA and Flare share such similar core concepts like topic-based authoring, single-sourcing, and content reuse, which make them confusing.   

### Similarities between DITA and Flare
The following table lists the similarities and differences between DITA and Flare.   
| Feature | DITA | Flare| 
|:---|:---|:---|
| Topic-based | Must strictly follow the predefined topic types (called "information types" in DITA): <ul><li>**Task**. Describes how to do something via step-by-step instructions.</li><li>**Concept**. Describes a general idea, definition, or principle.</li><li>**Reference**. Describes command syntax, programming instructions, and other reference materials. In DITA, images, video files, or other files that need to appear in a topic are inserted via a reference to them.</li></ul> | Optional. No strict requirement to follow any topic types. |
| Content reuse | Use conref, keys, profiling, and filtering with attributes to reuse content for multiple audiences or purposes. | Use snippets, variables, and conditions to reuse content for multiple audiences or purposes.|
| Authoring format | Strict XML | XML/HTML-based with MadCap tags|
| Multiple output formats| Supports HTML, PDF, and so on | Supports HTML, PDF, and so on | 

## Is Flare DITA?
Althouth Flare shares some core concepts with DITA, it does not mean Flare is DITA. The reasons are as follows:
- Flare is a tool that is proprietary to the MadCap company; while DITA is a standard that is not bounded to any tools. 
- Although both are topic-based, in DITA topics must strictly follow the information types to ensure that topics are semantically correct and correctly processed. Misuse of topic types may result in the loss of semantic power, strucutre formatting and validation.
- DITA strictly follows the XML format and uses the XML tags; Flare, also XML-based, supports HTML tags and MadCap XML tags. 

## How DITA works?
DITA is mainly made up of topics and maps. <br>
- **Topics**. Topics are content chunks that you can use in different deliverables. Topics come in, but are not limited to three core types. You can create more topic types. <br>
    - **Task**. Describes how to do something via step-by-step instructions. 
    - **Concept**. Describes a general idea, definition, or principle. 
    - **Reference**. Describes command syntax, programming instructions, and other reference materials. In DITA, images, video files, or other files that need to appear in a topic are inserted via a reference to them. 
- **Maps**. Maps are similar to table of contents. They are structures that define how topics are organized and presented in different deliverables, such as online helps and PDF files.
Topics are organized and using maps 

## Chracteriestics of DITA
DITA has the following characteristics:
- Topic-based. In DITA, you write content in chunks 
- Information type. 
- Content reuse. 
- Support dynamic information needs. 
- XML-based. 



## Is MadCap Flare DITA? 
MadCap Flare is an authoring tool that also features 
