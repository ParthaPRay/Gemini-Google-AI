
# Overview of Generative AI on Vertex AI

https://cloud.google.com/vertex-ai/docs/generative-ai/learn/overview

![generative-ai-workflow](https://github.com/ParthaPRay/Gemini-Google-AI/assets/1689639/c82ded2b-6d8b-43e1-a769-54f3ecad9be0)

* **Prompt**

The generative AI workflow typically starts with prompting. A prompt is a natural language request sent to a language model to elicit a response back. Writing a prompt to get the desired response from the model is a practice called prompt design. While prompt design is a process of trial and error, there are prompt design principles and strategies that you can use to nudge the model to behave in the desired way.

* **Foundation models**

Prompts are sent to a model for response generation. Vertex AI has a variety of generative AI foundation models (https://cloud.google.com/vertex-ai/docs/generative-ai/learn/models) that are accessible through an API, including the following:

1. Gemini API: Advanced reasoning, multiturn chat, code generation, and multimodal prompts.
2. PaLM API: Natural language tasks, text embeddings, and multiturn chat.
  Language support
Vertex AI PaLM API is Generally Available (GA) for the following languages. Vertex AI Gemini API also supports these languages.

Arabic (ar)

Bengali (bn)

Bulgarian (bg)

Chinese simplified and traditional (zh)

Croatian (hr)

Czech (cs)

Danish (da)

Dutch (nl)

English (en)

Estonian (et)

Finnish (fi)

French (fr)

German (de)

Greek (el)

Hebrew (iw)

Hindi (hi)

Hungarian (hu)

Indonesian (id)

Italian (it)

Japanese (ja)

Korean (ko)

Latvian (lv)

Lithuanian (lt)

Norwegian (no)

Polish (pl)

Portuguese (pt)

Romanian (ro)

Russian (ru)

Serbian (sr)

Slovak (sk)

Slovenian (sl)

Spanish (es)

Swahili (sw)

Swedish (sv)

Thai (th)

Turkish (tr)

Ukrainian (uk)

Vietnamese (vi)

   
4. Codey APIs: Code generation, code completion, and code chat.
5. Imagen API: Image generation, image editing, and visual captioning.
6. MedLM: Medical question answering and summarization. (Private GA)

The models differ in size, modality, and cost. You can explore Google's proprietary models and OSS models in Model Garden.

* Model customization

You can customize the default behavior of Google's foundation models so that they consistently generate the desired results without using complex prompts. This customization process is called model tuning. Model tuning helps you reduce the cost and latency of your requests by allowing you to simplify your prompts.

Vertex AI also offers model evaluation tools to help you evaluate the performance of your tuned model. After your tuned model is production-ready, you can deploy it to an endpoint and monitor performance like in standard MLOps workflows.

* Vertex AI Grounding service

If you need model responses to be grounded on a source of truth, such as your own data corpus, you can use grounding in Vertex AI. Grounding helps reduce model hallucinations, especially on unknown topics, and also gives the model access to new information.

* Citation check

After the response is generated, Vertex AI checks whether citations need to be included with the response. If a significant amount of the text in the response comes from a particular source, that source is added to the citation metadata in the response.

* Responsible AI and safety

The last layer of checks that the prompt and response go through before being returned is the safety filters. Vertex AI checks both the prompt and response for how much the prompt or response belongs to a safety category. If the threshold is exceed for one or more categories, the response is blocked and Vertex AI returns a fallback response.

* Response

If the prompt and response passes the safety filter checks, the response is returned. Typically, the response is returned all at once. However, you can also receive responses progressively as it generates by enabling streaming.


# Gemini-Google-AI

![Gemini_language_model_logo](https://github.com/ParthaPRay/Gemini-Google-AI/assets/1689639/5319a74a-4054-48b5-b26b-db8330f7b457)

Gemini, a family of multimodal large language models, was developed by Google DeepMind as a successor to LaMDA and PaLM 2. This family includes Gemini Ultra, Gemini Pro, and Gemini Nano, and was announced on December 6, 2023, positioning it as a strong contender against OpenAI's GPT-4.

The development of Gemini was announced by Google during the Google I/O keynote on May 10, 2023. Marking a significant advancement from its predecessor, PaLM 2, Gemini was still in early development stages at the time of announcement. Unique in its multimodal capabilities, Gemini was designed to process various types of data including text, images, audio, video, and computer code. This development was a collaborative effort between DeepMind and Google Brain, following their merger into Google DeepMind.

DeepMind CEO Demis Hassabis emphasized Gemini's capabilities in an interview, suggesting it could outperform OpenAI's GPT-4 and ChatGPT. This was part of Google's aggressive strategy to rival OpenAI, building on the success of DeepMind's AlphaGo. The model's development involved significant resources, including the involvement of Google co-founder Sergey Brin and a large team of engineers and legal experts.

Gemini's impending launch prompted OpenAI to accelerate its work on GPT-4, incorporating features similar to Gemini's multimodal capabilities. Google planned to make Gemini available through Google Cloud's Vertex AI service, and the model was set to power a range of Google products, including Bard and the Pixel 8 Pro smartphone.

At the virtual press conference on December 6, 2023, Pichai and Hassabis announced Gemini 1.0, comprising three models tailored for different applications. Gemini Ultra was poised for integration into Bard Advanced and availability to developers in 2024. Gemini Pro and Nano were integrated into Bard and the Pixel 8 Pro, respectively. Gemini was trained and powered by Google's Tensor Processing Units and was named in reference to the DeepMind-Google Brain merger and NASA's Project Gemini.

Gemini Ultra was reported to outperform several leading AI models, including GPT-4, and was the first to exceed human expertise in the MMLU test. Gemini Pro and Nano were set for wider availability to Google Cloud customers and Android developers. DeepMind also explored how Gemini could be combined with robotics.

The Gemini models share a common software architecture, with modifications for efficient training and inference on TPUs. Being multimodal, they can process multiple forms of input within each context window. Gemini's dataset is multimodal and multilingual, encompassing diverse data types.

The anticipation and speculation surrounding Gemini's launch were significant, with predictions of its impact on the AI landscape. Reactions to its unveiling were mixed, with some praising its potential and others comparing it to routine tech upgrades. Concerns were also raised about the demonstration of Gemini, highlighting the need for real-time verification of its capabilities.





![Screenshot 2023-12-30 123910](https://github.com/ParthaPRay/Gemini-Google-AI/assets/1689639/e9498629-c8f4-4895-8a54-9632a923bc17)




![Screenshot 2023-12-30 124134](https://github.com/ParthaPRay/Gemini-Google-AI/assets/1689639/1fd51f85-4cc6-4a91-8766-6dbbe8ca3deb)


# State-of-the-Art Performance of Gemini Ultra


* Broad Evaluation: The performance of Gemini models, particularly Gemini Ultra, has undergone extensive testing across a spectrum of tasks. These evaluations include understanding natural images, audio, and video, as well as complex mathematical reasoning.
Benchmark Excellence: In the realm of large language model (LLM) research and development, Gemini Ultra has surpassed the existing state-of-the-art results in 30 out of 32 widely recognized academic benchmarks. This achievement underscores the model's exceptional capabilities and versatility.

* Unprecedented Performance: A standout feature of Gemini Ultra is its record-breaking score of 90.0% in the Massive Multitask Language Understanding (MMLU) benchmark. This score is significant as it marks the first instance where an AI model has outperformed human experts.

* Comprehensive Subject Coverage: The MMLU benchmark encompasses an array of 57 diverse subjects, including mathematics, physics, history, law, medicine, and ethics. This broad scope is designed to assess not just world knowledge, but also the problem-solving abilities of the AI model.

* Advanced Reasoning Approach: Gemini Ultra's approach to MMLU is innovative in its use of reasoning capabilities. Unlike models that rely on initial impressions for responses, Gemini Ultra deliberates more thoroughly before answering complex questions. This method leads to more accurate and insightful responses, showcasing significant improvements over traditional AI response strategies.

* Technical Superiority: The remarkable performance of Gemini Ultra in such a wide array of benchmarks, particularly in surpassing human experts in MMLU, is a testament to its technical superiority. It indicates a significant advancement in the field of AI, pushing the boundaries of what AI models are capable of achieving.

* Enhanced Problem-Solving Abilities: The ability of Gemini Ultra to outperform in MMLU suggests a leap in AI's problem-solving abilities, especially in tasks requiring deep understanding and analytical thinking. This capability has profound implications for various applications where complex reasoning is essential.

* Future Applications: The success of Gemini Ultra in these rigorous tests opens the door to numerous potential applications. Its advanced reasoning skills can be pivotal in sectors like healthcare, legal analysis, scientific research, and more, where nuanced understanding and problem-solving are crucial.

![gemini_final_text_table_amendment_13_12_23](https://github.com/ParthaPRay/Gemini-Google-AI/assets/1689639/36972a24-733b-46cf-8395-24ff09394507)

![gemini_final_multimodal_table_bigger_font_amendment_lines](https://github.com/ParthaPRay/Gemini-Google-AI/assets/1689639/d2d4d425-14a3-4909-99a4-033df8421df1)



# Google AI Dev

https://ai.google.dev/


# Quick Start Guide

https://ai.google.dev/tutorials/ai-studio_quickstart


# Google Maker Suite Freeform prompt

https://makersuite.google.com/app/prompts/new_freeform



# Explore generative AI models in Model Garden

Model Garden is a platform that helps you discover, test, customize, and deploy Google proprietary and select OSS models and assets. To explore the generative AI models and APIs that are available on Vertex AI, go to Model Garden in the Google Cloud console.

https://console.cloud.google.com/vertex-ai/model-garden?_ga=2.246762944.536897531.1703956056-1538912965.1703920777


# Vertex AI Studio Platform

Enable Vertex AI API, if not enabled. It requires Billing.+

![Screenshot 2023-12-31 204840](https://github.com/ParthaPRay/Gemini-Google-AI/assets/1689639/34cb6dd3-880a-40d9-9311-b7cfe04cc0a5)


https://console.cloud.google.com/vertex-ai/generative?_ga=2.247808451.536897531.1703956056-1538912965.1703920777


# Gemini API Learning

https://cloud.google.com/vertex-ai/docs/generative-ai/model-reference/gemini


# ipynub Python SDK for Gemini and Overview

https://github.com/GoogleCloudPlatform/generative-ai/tree/main

https://cloud.google.com/vertex-ai/docs/generative-ai/learn/overview

https://github.com/GoogleCloudPlatform/generative-ai/blob/main/gemini/getting-started/intro_gemini_python.ipynb


# ModelGarden

https://cloud.google.com/vertex-ai/docs/start/explore-models

Various types of models to pick for business solution as on December 31, 2023.

![image](https://github.com/ParthaPRay/Gemini-Google-AI/assets/1689639/1881ac6c-4d99-47af-9f3a-9a7be102940c)



# **References**

1. https://en.wikipedia.org/wiki/Gemini_(language_model)
2. https://www.youtube.com/watch?v=36e74W1_-nw&ab_channel=GoogleCloudEvents
3. https://blog.google/technology/ai/google-gemini-ai/
4. https://deepmind.google/technologies/gemini/#introduction
5. https://blog.google/technology/ai/google-gemini-ai/?utm_source=gdm&utm_medium=referral
6. https://en.wikipedia.org/wiki/Gemini_(language_model)
