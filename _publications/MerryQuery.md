---
title: "MerryQuery: A Trustworthy LLM-Powered Tool Providing Personalized Support for Educators and Students"
collection: publications
authors: 'Benyamin Tabarsi, Aditya Basarkar, Xukun Liu, Dongkuan Xu, Tiffany Barnes'
permalink: /publication/2024-merryquery
excerpt: 'The potential of Large Language Models (LLMs) in education is not trivial, but concerns about academic misconduct, misinformation, and overreliance limit their adoption. To address these issues, we introduce MerryQuery, an AI-powered educational assistant using Retrieval-Augmented Generation (RAG), to provide contextually relevant, course-specific responses. MerryQuery features guided dialogues and source citation to ensure trust and improve student learning. Additionally, it enables instructors to monitor student interactions, customize response granularity, and input multimodal materials without compromising data fidelity. By meeting both student and instructor needs, MerryQuery offers a responsible way to integrate LLMs into educational settings.'
date: 2024-10-04
img: '/images/merryquery.png'
---

MerryQuery is an AI-powered educational assistant that utilizes retrieval-augmented generation (RAG) to provide students with tailored responses based on course materials.

This tool is designed to support both **teachers** and **students**
- Teachers can input course materials, and define data controls to prevent undesirable content generation.
- Students receive responses tailored to their previous interactions and course materials with references.

![image](/images/merryquery.png)

## Motivation

The goal of the MerryQuery agent is to allow teachers to automate answer questions from students as accurately as possible. By allowing the LLMs to access information from class materials designed by the teachers, they can be used to automatically answer questions from students that may be simple to answer or repetitive.

## Core Features

- Creating, editing, and deleting agent configurations.
- Creating and deleting chat sessions.
- Controlling access to agent configurations.
- Agent responses are tailored to individuals according to their account information.
- Student queries are visible to teachers.