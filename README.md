Designing an Agentic AI for ADHD Task Management Using the GDVRR Protocol

KMK3013 Knowledge-Based System

Group Members

- Stella Francis
- Shirley Jane Julian
- Clare Brooklyn Anak Akei
- Vailery Keling Katan
- Nataly Kinli

---

Project Overview

This project focuses on designing an Agentic AI assistant for ADHD task management using expert-derived knowledge obtained through a human expert interview.

The objective of the system is to help users:

- Manage tasks effectively
- Reduce feelings of overwhelm
- Improve focus and concentration
- Encourage task completion through structured support

The AI system was developed using Gemini/OpenAI and evaluated using the GDVRR Protocol:

1. Generate
2. Deconstruct
3. Verify
4. Rewrite
5. Reflect

Human Expert

- Darren Sebastian

Registered Counselor

- Lembaga Kaunselor Malaysia

The expert interview focused on:

- ADHD-related challenges
- Task management strategies
- Focus improvement techniques
- Communication approaches for ADHD support

Knowledge Engineering Process

Declarative Knowledge

Expert knowledge was converted into IF–THEN rules, including:

- IF a task is long, THEN break it into smaller steps.
- IF the user feels overwhelmed, THEN provide one or two simple starting steps.
- IF the user is distracted, THEN suggest timers or reminders.
- IF the user needs motivation, THEN provide supportive encouragement.

Procedural Knowledge

The following tools were designed for the AI assistant:

- Task_Chunking_Tool
- Focus_Timer_Tool
- Checklist_Generator_Tool
- Reminder_Tool
- Motivation_Tool

System Constraints

The AI assistant was instructed to:

- Use short and clear instructions
- Avoid medical advice or diagnosis
- Follow expert-derived rules and procedural tools
- Restrict unsupported reasoning structures

Agent Architecture

The AI system consists of three main components:

- Declarative Knowledge – Implemented as IF–THEN rules within the prompt template. These rules guide how the AI responds to different user situations.

- Procedural Knowledge – Implemented as predefined AI tools, including Task_Chunking_Tool, Focus_Timer_Tool, Checklist_Generator_Tool, Reminder_Tool, and Motivation_Tool.

- System Constraints – Implemented through the system prompt to ensure the AI follows expert-derived rules, maintains appropriate boundaries, and avoids unsupported reasoning structures.

GDVRR Analysis

Generate

The AI was tested using the following scenario:

"I have a 3-hour group assignment due tomorrow night. I feel very overwhelmed and I do not know where to start. I also keep getting distracted by my phone."

Deconstruct

The original execution trace contained:

- Stage 1 (Recipient/Intent)
- Stage 2 (Radioactive Vault)
- Stage 3 & 4 (Domain & Accuracy)
- Micro-tasking
- Environment Priming

Verify

The generated reasoning structures were not present within the expert-derived knowledge base, procedural tools, or system architecture.

KBS Anomaly Identified

Epistemic Boundary Violation (Knowledge Hallucination)

The AI generated unsupported reasoning structures and strategy labels that were not defined by the human expert.

Rewrite

To address the anomaly, a new declarative rule was introduced:

"IF the AI assistant generates reasoning structures, labels, or execution logic not explicitly defined in the expert-derived knowledge base, THEN reject and restrict them from being used."

The prompt template was revised to ensure that only predefined rules and procedural tools could be used.

Reflect

The GDVRR analysis demonstrated the importance of human oversight in identifying hidden reasoning errors and ensuring alignment between AI-generated outputs and expert-derived knowledge.


Repository Contents

This repository contains:

- Final_Report.pdf
- Original_Prompt.txt
- Revised_Prompt.txt
- Execution_Trace.txt
- Presentation_Slides.pdf
- Implementation screenshots


Conclusion

This project demonstrates how expert knowledge can be integrated into an Agentic AI system through knowledge engineering techniques. The GDVRR protocol successfully identified hallucinated reasoning structures and improved alignment between AI reasoning and deterministic expert knowledge through prompt refinement and human verification.
