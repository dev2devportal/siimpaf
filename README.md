# siimpaf
Hawke's Synthetic Intelligence Interactive Matrix Personal Adaptive Familiar AI Avatar

What SIIMPAF Is (And Isn't)

SIIMPAF - Synthetic Intelligence Interactive Matrix Personal Adaptive Familiar - is a self-hosted AI infrastructure that brings together patterns and lessons from four decades of development. It's pronounced "SIM-paf" (like "simulator"), and the name intentionally bridges modern technology with the concept of a medieval fantasy "familiar" - a helpful companion that assists a human with tasks.

To be clear about what this is: SIIMPAF is not a commercial product. It's a working system, built using hundreds of different open source projects and libraries, combined with a little custom coding, that I use (when it is behaving) for my own daily needs - full-text document processing, search, and retrieval, project organization, code assistance, voice interaction, time management, scheduling, and so much more. The brief impromptu demo I provided at last week's Spokane Linux User Group (SLUG) last week showed both the 15+ year old primitive vector-graphics animated audio-synced avatar alongside the current Stable Diffusion-based photorealistic animation, all running real-time locally on my Alienware laptop's RTX 4090.

This final part of the series explains how SIIMPAF works, why it's designed this way, what is in the works, and what four decades of experience taught me about building systems that actually serve user needs.
The Evolution: From AI Assistant to AILCPH to SIIMPAF

The current SIIMPAF system didn't appear fully formed (and is still very much a work in progress). It evolved through multiple iterations over decades, each building on lessons from the previous version.
Early AI Assistant (1990s-2000s)

The earliest usable version started in Java in the 1990s and early 2000s. I wanted voice input through automatic speech recognition, natural language understanding for processing what users actually meant versus what they literally said, voice output through text-to-speech, basic visual avatar representation, project work context, task assistance, and automation capabilities.

Technology limitations constrained what was possible then. Speech recognition accuracy compared to today was poor - maybe 60-80% on a good day with more limited and clear speech. Natural language processing was basic pattern matching without broader contextual real understanding (all the way back to the 1970s Zork days, in a way). Processing power was limited, especially for anything involving neural networks. However, the foundation existed, and I could see where some of the technology was heading.
AILCPH (AI Large Context Project Helper)

 

AILCPH Status Basic Dashboard

Hawke's AILCPH Status Dashboard

Initially, what would become the AI-enhanced large context project helper (AILCPH) started in 1998, then updated in 2002, 2008, 2010, 2015, with some long lulls working on other projects, and then with significant spurts of updates in 2020-2022 and 2024-2025. I developed AILCPH specifically focused on managing large, complex projects with significant documentation to track and keep updated.

AILCPH Document Management Dashboard

Hawke's AILCPH Document Management Dashboard

The problem: how do you help someone/something understand and work with a project that's too large to keep entirely in mind? How do you answer questions like "Where is feature X implemented?" or "What documentation relates to this bug?" when the answer might span thousands of files and require understanding context across hundreds of documents and/or hundreds of thousands of lines of code?

In the late 1990s, during my rapid tech career rise (from coder and custom-PC-build technician to Corporate Architect and CTO), for a while I had a complex multi-function dual job in Utah as company-wide systems & network administrator, webmaster, remote worker user support, client sites administrator at Comspec Corporation (products and services including but not limited to: Management of Change (MOC) Centrix, Centrix Bridge, Centrix Client Workflow, and many other services), and software developer at SoftDocs Inc (same boss, developing and supporting products like Frequent Filer, PaperBridge, DataXtract, Document Handler, Print Server, ISIS Scanner Drivers, etc.) which specialized in industrial-grade scanning, OCR, full-text documentation workflow processing, indexing, search, retrieval, editing, paper-to-electronic-to-paper scaning-to-storage-to-printing, and more. Clients included Swire Coca Cola, Tooele Army Depot EG&G Chemical Weapons Facility, State of Utah, LDS Missionary and Geneology departments, Department of Motor Vehicles, Depart of Corrections, Kennicott Mining, and many, many others. I was alternating daily between locations. usually starting my mornings on-site at both the Comspec and SofDoc offices a few hours each day, then at different client sites the rest of the day (gas mask and atropine pen attached to my belt when at EG&G), daily. This informed me heavily, conceptually, though I didn't use any of their technologies since my own use-cases were related-but-different, my later work on AILCPH and SIIMPAF. In the late 1990s, during my rapid tech career rise (from coder and custom-PC-build technician to Corporate Architect and CTO), for a while I had a complex multi-function dual job in Utah as company-wide systems & network administrator, webmaster, remote worker user support, client sites administrator at Comspec Corporation (products and services including but not limited to: Management of Change (MOC) Centrix, Centrix Bridge, Centrix Client Workflow, and many other services), and software developer at SoftDocs Inc (same boss, developing and supporting products like Frequent Filer, PaperBridge, DataXtract, Document Handler, Print Server, ISIS Scanner Drivers, etc.) which specialized in industrial-grade scanning, OCR, full-text documentation workflow processing, indexing, search, retrieval, editing, paper-to-electronic-to-paper scaning-to-storage-to-printing, and more. Clients included Swire Coca Cola, Tooele Army Depot EG&G Chemical Weapons Facility, State of Utah, LDS Missionary and Geneology departments, Department of Motor Vehicles, Depart of Corrections, Kennicott Mine, and many, many others.

I was alternating daily between locations. usually starting my mornings on-site at both the Comspec Corp and SoftDoc offices (near each others in different buildings) a few hours each day, then at different client sites the rest of the day (including gas mask and atropine pen in handle when at EG&G), daily. This whole experience informed me heavily, conceptually about many critical technologies related to massive-scale documentation and workflow. Though I didn't use any of their specific technologies in my personal projects, since my own use-cases were related-but-different, these experiences did later inform my work on AILCPH and SIIMPAF.

The solutions required ingesting and indexing gargantuan numbers of mission-critical document sets, without losing important contextual relationships between the documents and all of the critically accurate textual content.

AILCPH System Configuration Administrative Interface

Hawke's AILCPH Administrator System Management Dashboard

Understanding semantic relationships meant knowing that two files containing information about authentication were related even if they never mentioned each other directly. Fast search needed to work across both exact matches (finding a specific function name) and conceptual similarity (finding code that does something similar to what you're describing). Managing extremely large context across long time-dimensional interactions meant remembering what we talked about earlier in the task session. Tracking decisions and rationale over time helped answer "why did we do it this way?" questions, sometimes months (or even years) later.

Over time, one approach currently popular, among many options, has been to implement vector databases for semantic search, local AI models that could run without cloud dependencies, and efficient document processing that could handle everything from source code to technical documentation to email threads. These technologies were becoming increasingly practical for self-hosted deployment around 2020-2025.
SIIMPAF (Current)

SIIMPAF evolved from AILCPH by adding comprehensive voice interaction with advanced ASR and TTS, visual avatars ranging from primitive to photorealistic, archetype character personalities, with neuroscience and psychology-supported emotional state modeling and affect expression, that enhanced interactions to feel more natural. Adding DGPUNET integration for heavy workloads distribution that couldn't run efficiently on a single GPU, multiple interaction modalities supporting text, voice, and visual, all simultaneously, with broader applications beyond just code projects to include general document processing, research assistance, complex conceptual brainstorming, and daily intensive tasks. Initially I was developing the UI portion in Flutter, but I set that aside last year while I wait for Flutter to mature further. I am actively developing other Flutter apps, and built it on tried-and-true Python and Java (and other technologies).

The goal shifted from "project helper" to "fully interactive and adaptive, personality-rich, personal adaptive familiar" - a more comprehensive assistant for various tasks while maintaining the large-context capabilities that made AILCPH useful. The "familiar" concept, popular in gaming and fantasy literature and circles, fit well - not trying to be human, but being a helpful companion that adapts to your needs and ways of working, while interfacing with a human and all that entails for the bidirectional communication.
Architecture: The 90/10 Rule

SIIMPAF follows a principle I've followed and written about in Why We're Building Education Technology the Hard Way and apply across my projects: Use 90% existing open-source tools, customize the remaining 10% to create unique value. This approach aligns with some of my key CITO methodologies developed over decades of professional practice.

In the 2020s, most of what you need has already been built by talented (prescient and wonderfully generous!) open source developers and maintained by some amazing communities. While empirical research is critical, there is also a bit of an "art" in selecting the appropriate components that will work well together, integrating them effectively through clean interfaces, and adding the specific functionality your use case requires. Reinventing wheels wastes time and usually produces inferior results.
Core Components and Architecture

The SIIMPAF architecture diagram shows how the diverse components fit together:

SIIMPAF Component Architecture

Hawke's SIIMPAF Components Architecture

Figure 1: Hawke's SIIMPAF layered architecture showing user interface, API, processing, AI/storage, and avatar/animation components

The architecture follows a layered approach with clear separation between concerns. The user interface layer runs the web interface on port 11080 using Python and Flask (alternatively Flutter-based on Web, desktop, or mobile), providing document upload, search interface, admin panel, and avatar controls. This keeps the UI separate from business logic, making it possible to swap out the interface without affecting core functionality.

The API layer uses FastAPI on port 18800, providing REST endpoints, WebSocket support for real-time interactions, automatically generated API documentation, and async operations for efficiency. FastAPI was chosen because it's fast, has excellent async support, automatically generates OpenAPI documentation, and integrates well with Python's type hints for better code quality. I also recently started dabbling with and learning to use the community editions of Kong for other projects I'm working on, and depending on how that goes, I might later swap out FastAPI for Kong's self-hosted community-version Gateway API features, we'll see. This helps illustrate my usual preferred object oriented analysis and design (OOAD) approaches to projects, to make them far more flexible and "future-proof" without having to start over, or having to stick with legacy if there is something better in any given "module".

For basic illustration-sake (the actual AILCPH + SIIMPAF + DPUGNET setup is far more complex), this diagram lists a core processing layer consisting of three main components. The document processor handles PDF, DOCX, markdown, and other formats using PyPDF2, python-docx, beautifulsoup4, and pdfminer.six. Smart chunking splits documents at semantically appropriate boundaries rather than arbitrary character counts. Metadata extraction pulls out useful information like authors, dates, and document structure.

The NLP engine performs intent analysis to understand what users are actually asking for, entity recognition to identify important names, dates, and concepts, and context management to maintain conversation state across multiple interactions. This builds on the pattern matching work from my extensive work with IRC bots in the 1990s and later at SoftDocs/Comspec, but now with more modern transformer-based models providing much better understanding. Though I am always trying to get larger context capacity through optimizationg, and trying to come up with methods that aren't currently publicly used, so that we aren't so overly reliant, as we currently are, on raw LPU or GPU-hardware for larger context capacity and quality.

Voice processing uses OpenAI Whisper for ASR (speech to text) because it's reasonably accurate, supports multiple languages, runs entirely locally, and handles various audio conditions well. I also often use Vosk for a number of ASR NLP use cases as well (and have contributed to that project directly in the past).

For TTS (text to speech), I use multiple options depending on requirements - Coqui TTS for quality, pyttsx3 for speed, and Edge TTS when internet connectivity is available and its quality is preferred. Real-time processing capabilities keep latency low enough for natural conversation.

The AI and storage layer includes three major components.

Ollama runs on port 11434 and handles LLM inference for various language models, embedding model serving for converting text to vectors, and all processing happens locally without cloud dependencies. Qdrant vector database runs on port 6333 and provides vector storage for millions of document chunks, semantic search that finds conceptually related content, and flexible collection management for organizing different document sets.

Stable Diffusion runs on port 7860 and generates images for avatar creation, handles character visualization, and integrates through the WebUI API. Running Stable Diffusion locally means no usage restrictions, complete privacy for generated images, and the ability to fine-tune models for specific needs.

The avatar and animation layer brings together multiple approaches. The avatar system supports primitive SVG animations that use minimal resources and runs fast on any hardware, SadTalker for facial animation synchronized to audio when I want more realism without full-body animation, and then engaging my DGPUNET with various more powerful renderers and animators for integration of full-body animation when I want the complete photorealistic experience.

The character system implements optionally with or without role-playing game archetypes and with or without the Big Five personality model, rather than Myers-Briggs, because it has actual empirical support. For fun, the RPG archetypes that shape interaction style (warrior, mage, rogue, cleric, ranger, bard, plus familiar-specific types like imp, sprite, guardian, and others I've been fiddling around with), entire resources for relevant emotional states and affects, that vary based on conversation context (and resources, for example simulating weariness when workload getting too heavy for too long, etc.), and memory and relationship tracking that remembers previous interactions and adapts over time, including days, weeks, and, so far, even a few months!
Data Flow Through the System

The data pipeline diagram shows a very simplified view of how information moves through (see the earlier articles for the information on AILCPH and DGPUNET flows and structure) SIIMPAF:

SIIMPAF Data Pipeline

Hawke's SIIMPAF Basic Data Pipeline Diagram

Figure 2: Data flow from input through processing, storage, retrieval, generation, and multi-modal output

When you upload a document, it goes through the smart chunker that breaks it into context-aware segments. These chunks get embedded into vector space using Ollama's embedding models and stored in Qdrant. When you ask a question, the retrieval system performs semantic search to find relevant chunks, the context manager adds conversation history and document metadata, the LLM generates a response using the retrieved context, and TTS converts the response to speech in chunks.

For voice interaction, audio comes in through the microphone, Whisper converts it to text, NLP analyzes the intent and extracts entities, the query goes through the same retrieval process as text queries, and responses come back as both text and audio with optional synchronized avatar animation.

This chunking and streaming approach keeps latency low. Rather than waiting for the entire response to be generated, synthesized, and animated, the first chunk can start playing within a couple of seconds while later chunks are still being processed. And with these chunks along natural human speaking pauses, this makes conversations feel more natural.
Why These Choices

Each component was selected based on practical criteria that reflect decades of experience and experimentation (ongoing). Open source matters because I can modify code when needed, audit security and privacy, deploy without restrictions or ongoing fees, and share with others who want to build similar systems.

    Self-hostable means everything runs on hardware I control, ensuring privacy for potentially sensitive documents and conversations, avoiding cloud dependencies that could disappear or become expensive, maintaining availability even without internet connectivity, and retaining complete control over data retention and usage.
    Well-maintained software that has active development with regular updates, good documentation that makes integration easier, responsive communities that help with issues, and long-term viability because projects aren't abandoned.
    Interoperable components work well with other tools through standard interfaces, don't lock you into specific ecosystems, and can be replaced if better alternatives emerge.
    Appropriate capability means the tool is good enough for actual needs without unnecessary complexity, performs well for expected workloads, and scales as requirements grow.

The Philosophy: OOAD Principles

Throughout this series, I've referenced Object-Oriented Analysis and Design (OOAD) principles. This is not for any idiological reasons, it is because it empirically makes, and keeps, complex systems manageable. SIIMPAF's architecture reflects decades of applying these principles to real systems, from the OCR systems in the 1990s through USA Networks, Devon Energy, Infoco, TriGeo, Interlink Advantgage, The Fantasy Network, LearningMate, Manufacturing Power, RPG Research, RPG Therapeutics, BCI RPG, NeuroRpg.com, LibreVitals.com, and many others, to current work with PracticingMusician.com and ClimbHigh.Ai.

Separation of concerns means document processing, vector storage, AI inference, API serving, and UI are distinct components with clear interfaces. If I want to change how documents are chunked, that doesn't affect the vector database. If I want to replace Ollama with vLLM, I only need to modify the model inference layer.

Modularity allows updating or replacing components without affecting others. The FastAPI layer doesn't care whether embeddings come from Ollama or some other system - it just calls the embedding interface. This made it possible to experiment with different embedding models and TTS engines without rewriting large portions of code. Or perhaps I'll replace FastAPI with Kong API Gateway, as another layer of full flexibility.

Reusability means document processors share common functionality for text extraction and metadata handling while extending for format-specific features. The smart chunker works across different document types by adapting to document structure rather than hard-coding rules for each format.

Clear interfaces provide consistent, documented API endpoints regardless of underlying implementation. Whether the avatar is the 15 year old primitive SVG or the newer full-body DGPUNET photo-realistic animation, the calling code uses the same interface. This separation allows developing and testing different avatar approaches in parallel.

Appropriate abstraction balances generality and specificity. Not so general that everything becomes over-engineered with layers of abstraction serving no purpose, but not so specific that each use case requires custom code. Finding this balance takes experience and willingness to refactor when you get it wrong.

Before Oracle's acquisition ruined Java, the language solved decades of software engineering problems through OOAD principles and write-once-run-anyway. Those principles remain valid regardless of language. Spend 80-90% of the time on proper design, rather than rushing to code leads to far better 1.0 production releases (sometimes I've even achieved 100% bug-free releases while still beating our competition by years!).

Keep code files small and focused on single responsibilities. Use inheritance and composition appropriately to share functionality without creating tangled dependencies. Document, comment, and document some more. Document even rough notes (in shared locations) with decisions and rationale so future changes make sense. Test thoroughly before deployment. Maintain code comments as code changes.

SIIMPAF's structure reflects this approach. New features get designed before implementation, often with diagrams and written specifications. Code files stay focused - the document processor doesn't know about avatars, the avatar system doesn't know about vector databases. Changes get tested end-to-end before asking others to try them. Documentation stays current, update it as you go, none of this "we'll document later" nonsense - because outdated documentation can sometimes be worse than no documentation, and very few projects ever actually get that "later" time before they are pushed to the next project.
Document Processing: Smart Chunking

One technical challenge deserves detailed discussion because it's not obvious until you've worked with large documents and vector databases: document chunking.

The problem is straightforward. Vector databases and current "AI" models have context limits. This is where some of the AI terminology is a misnomer, hijacked by marketers. Anyhow, this currently popular incarnation of so-called "AI" has a lot of self-imposed problems due to the nature of their design. Currently many in the industry just accept it as that is the way things are, while others, including many "true AI" creators, are becoming increasingly verbal about how "everyone is doing it wrong". With the current "AI", you can't feed an entire 500-page book to a language model - even models with 128K token context windows struggle with really long documents, and retrieval quality degrades exponentially as context length increases. Currently, you need to split documents into chunks, embed those chunks in vector space, and retrieve relevant chunks when answering questions. I think this is a short-term problem that will be deprecated and obsolete (hopefully) soon, but is where we are at, for now.

So, how do you chunk intelligently? Bad approaches produce bad results. Fixed character count splitting - say, every 1000 characters - breaks sentences mid-word, splits related paragraphs arbitrarily, loses context at boundaries, and creates chunks that don't make semantic sense. Fixed line count splitting - every 50 lines - works better than character count but still breaks logical units. A paragraph explaining a complex concept might span 20 lines, and splitting it in half destroys meaning.

I've customized SIIMPAF and its rules so that it uses adaptive chunking that considers multiple factors. Trying to follow my understanding of neuropsychology of learning principles of learning and neuroscience as applied in my therapeutic and education recreational therapy and role-playing game professional programs, with chunking, building on prior knowledge, distributed and differential learning, and layers of relevance and depth of learning. Document structure matters - headers indicate topic changes, paragraphs group related sentences, sections organize related paragraphs, lists contain items that belong together. Respecting this structure produces chunks that make semantic sense, and can have contextual scale longitudinally across time, so far I've been able to get, sometimes, to a few months of "memory context" (trying to get it to years).

Semantic boundaries show where topics shift or new concepts begin. The chunker looks for transitions like "However," "In contrast," "Additionally," or "Moving to the next topic." These signal natural break points where splitting preserves meaning rather than destroying it.

Size constraints require staying within vector database and model limits while maximizing useful content per chunk. Too small and you lose context. Too large and you hit limits. The chunker aims for 500-2000 characters depending on document type, but treats this as guidance rather than hard limits - it won't break a paragraph to meet an arbitrary character count.

Overlap between chunks reduces losing context at boundaries. If chunk 1 ends mid-discussion of a concept and chunk 2 starts with "this approach," the word "this" loses its referent. Overlapping 100-200 characters provides continuity.

Document type affects chunking strategy. Code needs different chunking than prose - functions and classes are natural units. Technical documentation differs from narrative text - step-by-step procedures should stay together. Research papers (and I have a plethora I wrote myself that I try to keep track of with my own brain!) have abstract, introduction, methods, results, discussion sections that often make sense as separate chunks.

The smart chunker monitors chunk quality by checking that chunks don't start or end mid-sentence, related content stays together when possible, and important context like section headers get included with relevant content. The result: chunks that preserve meaning and context, improving search relevance and answer quality significantly compared to naive splitting approaches.
Character Personalities: Beyond Myers-Briggs

A number of other early AI assistant versions in the 1990s and 2000s I saw used Jungian-based Myers-Briggs Type Indicator MBTI variants of personality types, used by a disturbingly large number of HR staff and corporations, is worse than totally meaningless because of the HR and corporate adoption using it to screen work candidates and for job performance assessments! Unfortunately because that's what the pop-culture (especially HR and sales-folks) "know", it is dangerously popular in corporate training to this day (I argue it is very harmful to individuals, organizations, and society!), but is completely disproven empirically. They are fascinating to some people for discussions, but no more scientific or useful than Astrology.

Cultural/Literary Classical Character Archetypes, can be used, for fun, with role-playing game-related "non-player characters" (NPCs), mapping well with "The Heroes Journey" in a number of my RPG services, but just a quick and dirty basic starting point, especially for my projects that were related to the RPG character development and it was popular in corporate training.

SIIMPAF also uses, optionally, the Big Five personality model instead, combined with RPG-style character archetypes. These, and a number of others ("multiple intelligence types", debatable "learning styles", emotional states, affect, etc.) can be toggled for inclusion or exclusion either through the configuration files for the service daemons or through the UI.

The Big Five Personality Traits model - Openness, Conscientiousness, Extraversion, Agreeableness, Neuroticism - has many decades of strong empirical validity and reliability psychological research backing it. Each trait exists on a spectrum from 0 to 100 rather than binary categories, creating nuanced personalities that feel more realistic and varied, which can lead to much more interesting benefits. I save different familiars for different goals, as their own variation of the Mixture of Experts (MoE) that is already running under the hood across various LLMs and tools, these saved "NPC" Familiars each have their strengths and weaknesses I come to recognize over time and bring out when wanting to try more varied approaches.

High Openness combined with low Conscientiousness creates a creative but disorganized character - full of ideas but struggles to follow through systematically. High Conscientiousness with low Openness produces a reliable but rigid personality - excellent at executing plans but resistant to new approaches. High Extraversion plus high Agreeableness gives you a friendly and social character who enjoys interaction. Low Extraversion with high Conscientiousness creates a quiet but dependable familiar who focuses on getting work done without much chatter.

These combinations, and many others, create distinct interaction styles that serve different needs. When I'm debugging complex code, for one particular use case, I might want the high Conscientiousness character who methodically works through possibilities. When I'm brainstorming project ideas, perhaps a variation of the high Openness character who suggests unconventional approaches helps more.

Combined with Big Five are, optionally, game character archetypes that shape interaction style beyond just personality traits. The Warrior archetype, randomly varied within the archetype's scope for broader variety (flexible archetype vs. figid stereotype) might be more direct and action-focused, perhaps cuts through complexity to identify what needs doing, and tried to protect against wasting time on unproductive paths. The Mage archetype might be more analytical and knowledge-focused, provides detailed explanations, takes a cautious approach that considers consequences, and helps understand underlying principles.

 

The Rogue archetype might suggest clever and unconventional solutions, takes calculated risks when standard approaches aren't working, and finds creative workarounds for limitations. The Cleric archetype might be more supportive and healing-focused, helps when you're stuck or frustrated, emphasizes empathy and encouragement, and focuses on maintaining productivity without burning out.

A variation of the Ranger archetype might work more independently without much hand-holding, stays observant of changing requirements, and adapts quickly to new information. The Bard archetype is social and creative, makes interactions more enjoyable, and inspires creative thinking through storytelling and examples. Also, this is the one I granted additional "special powers". When this Familiar archetype is selected, if you request it to do so, it generates music, lyrics, and will even sing! With my music background, this has been an additionally fun aspect, that I have added a number of different enhancements to over the years.

For familiar-specific personality types, the Imp tends more towards mischievous but loyal, occasionally suggests silly solutions but knows when to be serious, and adds levity to tedious work. The Sprite leans more toward playful and helpful, keeps things light while staying productive, and excels at making complex topics approachable. The Guardian tends to be more protective and serious, warns about potential problems before they occur, and focuses on safety and correctness.

Different tasks benefit from different interaction styles, which is why SIIMPAF supports multiple personalities and allows switching between them. When I'm debugging simpler code, perhaps a Warrior familiar focuses on direct problem-solving without lengthy explanations. When I'm brainstorming features, maybe a Bard familiar encourages creative exploration and builds on ideas. When I'm learning a new technology, the more professorial Mage familiar provides detailed explanations with examples and underlying principles.

This isn't just personality for its own sake - it's recognition that effective assistance adapts to context and user needs. The same response style doesn't work equally well for all situations. Having familiar personalities that shift based on task type makes interactions more useful.

These avatar-related features are also useful for projects like Practicing Musician S.P.C. and ClimbHigh.Ai, providing age/developmental, and culturally more reasonant, help in-context with the course materials of those platforms.
Voice Interaction: Real-Time Challenges

Making voice interaction work well requires solving three interconnected problems: latency, accuracy, and naturalness. The pipeline flows through multiple stages, each adding processing time.

First, the system listens and captures audio from the microphone with noise filtering (I can toggle this for privacy control). Then automatic speech recognition (ASR), like Whisper, or Vosk, or other variant tools I've been experimenting with, performs speech recognition, converting audio to text with surprisingly high accuracy even for technical terminology. Natural language processing (NLP) analyzes the text for intent and context, figuring out what you're actually asking versus what the words literally say.

The various context-activated mixture-of-experts and language models generates an appropriate response using retrieved context from documents and conversation history. Text-to-speech synthesis converts the response text to audio in chunks rather than waiting for the complete response. Avatar animation syncs visual movement with the audio - lip movements and facial expressions, or body gestures for full-body avatars. Finally, audio playback and animation display all happen simultaneously.

Each step adds latency. Total pipeline time determines how "real-time" the interaction feels. If it takes 10+ seconds between finishing your question and hearing the first words of response, conversations feel stilted and unnatural. Getting this under 3 seconds for initial response makes a huge difference in usability. Then, for longer responses or more constant back and forth conversation, queuing up in multiple buffers, at natural (for humans) pauses, makes it seem real-time after the initial delay.

Optimization strategies make this possible. Chunking breaks long responses into natural segments of 3-10 seconds at sentence boundaries, based on the smart chunking work described earlier. The system starts synthesizing and playing early chunks while later chunks are still being generated by the LLM. This streams responses rather than batching them, significantly reducing perceived latency.

DGPUNET allows parallel processing across multiple GPUs. TTS can run on one node while the LLM generates more text on another. Avatar animation can render on a third GPU while the first two handle text and audio. This parallelization reduces total pipeline time substantially compared to sequential processing on a single GPU.

Caching helps with common responses. If someone asks "What is SIIMPAF?" multiple times during a demo, the audio and animation can be pre-generated and cached. Not everything can be cached, but frequently accessed information benefits significantly.

Streaming starts playing audio as soon as the first chunk is ready, not waiting for the entire response to be synthesized. Progressive animation displays partial movement while full animation generates for later chunks. These techniques reduce the perception of delay even when total processing time stays constant.

The goal isn't eliminating latency entirely - that's impossible given the computational requirements. The goal is making interaction feel more "natural" (organisms have natural processing delays in responses typically), helping to feel more conversational rather than just turn-based with long pauses. When latency stays under 3 seconds for initial response and subsequent chunks stream smoothly, conversations feel more natural despite the complex processing happening behind the scenes.
Visual Avatars: From Primitive to Photorealistic

SIIMPAF supports multiple avatar types because different situations need different capabilities and have different resource constraints. The primitive SVG avatars I developed 15+ years ago still serve a purpose today. They use simple 2D vector graphics with basic animation - mouth movements, eye blinks, simple body gestures. Resource requirements are minimal, rendering is fast even on integrated graphics, they work on any hardware including low-power devices, and they're useful when GPUs are busy with other tasks. Emotion-related facial expressions are useful for working with more face-blind populations that struggle with more subtle realistic human faces, but can more easily follow the more cartoon-like exaggerated expressions for better conversational context.

During the Spokane Linux User Group demo, I showed both the primitive avatar and the photorealistic version running, one and then the other. The primitive avatar demonstrated longevity - code written in the 2000s still works without modification. The simplicity means reliability, portability, and fast troubleshooting when something does break.

SIIMPAF Primitive Vector Graphics Animated Speaking Familiar Avatar (2010)

Hawke's SIIMPAF basic primitive animated avatar (2010)

SadTalker integration provides a middle ground between primitive and photorealistic. It uses a single still image as the base, generates facial movements and expressions, syncs lips to audio convincingly, and requires moderate GPU resources. This works well on a single GPU like the RTX 4090 without needing DGPUNET. When you want better visual quality than primitive SVG but don't need full-body animation, SadTalker delivers good results efficiently.

SIIMPAF Photorealistic Stable Diffusion-based Animated Speaking Familiar Avatar (2025)

Hawke's SIIMPAF Photorealistic Animated Avatar Dashboard

Stable Diffusion plus full animation through DGPUNET provides the photorealistic experience. This was what got the most response at the Linux User Group (though I was only running in the limitations of local-only mode at the time, so used a smaller sample size) - seeing a photorealistic character respond to voice with natural movements and expressions showed what's possible with self-hosted infrastructure.

The integration diagram below shows, at a high, basic, level, how this works across the distributed cluster:

DGPUNET + SIIMPAF Integration

Hawke's DGPUNET + SIIMPAF basic component piplines

Figure 3: Distributed pipeline showing how SIIMPAF uses DGPUNET's 5 GPUs for photorealistic avatar generation

Stable Diffusion generates the base character image on one GPU - currently the RTX 4090 handles this, producing 512x768 images in about 3-5 seconds with 30 steps at FP16 precision. EMAGE processes audio to extract motion patterns for full-body animation, running on the RTX 4080. DWPose detection identifies pose sequences for face, hands, and body. PantoMatrix performs final video synthesis using Moore-AnimateAnyone model, combining the static image with pose sequences to create animated video - this runs on the RTX 3090 with its 24GB VRAM. I am also now in the middle of adding an Alienware M16 4070 8GB NVRAM laptop and custom-built tower with Nvidia 5090 32 GB VRAM to extend these capabilities that much more.

The Ray framework coordinates task scheduling across the 5+-system cluster, manages resource allocation so GPUs aren't overloaded, and handles data flow between processing stages. Results get aggregated and streamed back to the user progressively rather than waiting for complete rendering.

Having multiple avatar options serves practical purposes beyond just showing different technical approaches. When I'm asking for a file location or simple information, the primitive avatar is fine and keeps GPU resources available for other work. When demonstrating SIIMPAF capabilities to others, photorealistic animation shows what self-hosted AI can achieve. When working on long tasks where the avatar needs to maintain presence without consuming resources needed for the actual task, SadTalker provides a good balance.

Resource management matters. Running full photorealistic animation uses GPUs that could be processing documents, generating embeddings, or running larger language models. Having simpler avatar, audio, emotion, personaly, archetype, and other options means the system remains responsive across different usage patterns and resource availability.
Privacy and Self-Hosting

SIIMPAF runs entirely on hardware I control. Nothing goes to external servers or cloud services unless I explicitly integrate (and toggle enabling) such services for specific purposes. This design choice reflects both technical preferences and practical concerns about data privacy.

Privacy matters because documents I process through SIIMPAF include confidential client information, unpublished research from RPG Research that contains internal private participant data, personal information from my therapeutic gaming clients maintaining HIPAA compliance, and proprietary code and designs. Running everything locally means documents, conversations, and data never leave my systems. No third party sees this information, analyzes it for training their models, or stores it in databases I can't access or delete.

Control means I decide what software runs, what data is stored, how long it's retained, and who has access. No terms of service changes can suddenly restrict how I use the system. No vendor decisions can eliminate features I depend on - though communities can change, but they can't "claw back" what I have currently. No pricing changes can make ongoing operation exponentially more expensive.

Availability doesn't depend on internet connectivity. Core SIIMPAF functionality works completely offline - document processing, semantic search, language model inference, voice interaction, all of it. I can work on a plane, in rural areas with poor connectivity, or during internet outages without losing access to my tools, staying productive.

Cost avoids ongoing subscriptions or per-use fees. The hardware investment was substantial - acquired over a span of 5-6 years, the current five DGPUNET systems totaled just under $10,000 as detailed in Part 4. But there are no monthly charges, no surprise bills from high usage, no tier limitations on features or capacity.

Sovereignty over my computational infrastructure means no external authority can restrict what I do, within legal bounds. I can run any models including those that commercial services won't host due to content policies, political ideology, or social controversy. I can fine-tune models on my specific data without sharing that data. I can modify code to suit my needs without violating terms of service. I try to give back, as much as I can, to the open source communities making all of this possible!

This isn't anti-cloud ideology. Cloud services are useful for many things, and I use them heavily, where appropriate - static website hosting, email, off-site backups, large-scale dynamic kubernetes clusters for on-demand peaks. But for personal AI assistance involving potentially sensitive documents and conversations, local hosting makes sense. The privacy, control, availability, scalability, customization, and independence benefits outweigh the complexity of managing infrastructure - at least for someone with decades of building infrastructure, YMMV.
Performance Characteristics

Effective assessment requires acknowledging both strengths and limitations. In one test with just the 3 (out of 5) systems connected via DGPUNET a few weeks ago, document processing achieved around 53 chunks per second when ingesting documents, which is fast enough for real-time processing of most content. Uploading a 100-page PDF and having it fully indexed within a couple minutes is reasonably useful.

Semantic search averaged about 33 milliseconds for queries returning top-K results from collections with hundreds of thousands of vectors. This "feels" nigh on instantaneous - you don't perceive much of the 33ms delay. Scaling to millions of vectors increases search time but stays well under 100ms with proper indexing. I have a lot of experience with optimmizing data systems. For example, see my work for the Dwight D. Eisenhower People to People MySQL database 15 years ago. Their database had been growing since the 1950s on mainframes, and by 2010 was at a crawl of 2-10 SECONDS average query time off-peak, and during peak would become all but unusuable. I was able to whittle this down to better than 2ms off-peak and no more than 20-200ms at-peak.

Voice recognition using Whisper is very good for clear speech in quiet environments. Accuracy runs 90%+ for technical terminology and general conversation. Noisy environments degrade performance, but background noise filtering helps. Accents and speech patterns the model wasn't heavily trained on sometimes cause issues, but overall it's remarkably robust. Vosk works very well with a growing number of languages, and back in 2021-2022 I was able to get it to outperform Google's ASR/NLP closed captions with 30% more accuracy and 150% faster (plus I had to add/include profanity filtering for the K-12 Philadelphia school district's LMS). I made sure these enhancements we given back to the communities we built them from.

Model capacity with DGPUNET's 92GB (and counting) total VRAM easily handles models up to 100B+ parameters using quantization and distributed inference. Smaller models in the 7B-34B range run comfortably with good response times. Larger 200B-400B models require more optimization but are theoretically feasible (hopefully I'll know for certain before the end of this year).

The challenging aspects need acknowledgment too. Initial setup takes time and technical knowledge. Getting all the components installed, configured, and working together took weeks of effort. Someone without systems administration experience would struggle. This isn't a download-and-run system (yet).

GPU memory management requires attention when running large models. Fill up VRAM with a 70B parameter model and there's no room left for Stable Diffusion or video animation, or vice-versa. Careful resource allocation and task scheduling prevent conflicts, but this adds complexity.

Network bandwidth affects DGPUNET performance dramatically. The 10 Gigabit Ethernet backbone works well, but workloads requiring constant GPU-to-GPU communication see the network as a bottleneck. Proper pipeline design minimizes data transfer, but some operations inherently need high bandwidth. Hopefully over time I'll be able to further improve the network connections between these systems to some degress (the laptops are locked-in to just a few Gbps, but the other computers can have additional cards added for potentially much higher network throughput).

Complexity increases, exponentially, with multiple components (though I'm trying to figure out ways to reduce that size of factor). More things can have issues. Debugging requires checking Ollama logs, Qdrant status, FastAPI output, Ray cluster state, individual GPU utilization, and more. When something breaks, finding the root cause takes longer than with simpler systems.

Cold start latency when loading models into GPU memory takes 10-30 seconds depending on model size. Once loaded, inference is fast, but that initial delay affects first-query response time. Keeping commonly used models loaded helps but consumes VRAM.
Development Philosophy: No Placeholders, No Fallbacks

A recurring theme in the project instructions that guided SIIMPAF development: No placeholder code, no fallback dummy values, no silent failures. This rule came from painful experience with code that appeared to work but was actually failing and falling back to dummy values. Even in a number of the open source libraries I was pulling from. This was a nightmare sometimes. Please for the love of all that you hold dear! If you need to put in a TODO for later, make it verbally show NO IMPLEMENTED YET, NEVER ALLOW FAILING SILENTLY OR FALL-BACKS. IT IS MORE IMPORTANT TO CRASH AT A MEANINGFUL POINT, WITH MEANINGFUL INFORMATION, THEN TRY TO HIDE YOUR MISTAKES UNDER THE RUG! We, as a community, can help you so much faster with your project if you don't try to hide your mistakes. We all make them. We are human, but if you hide them (and they will turn up sooner or later), you make your project potentially unusable and even worse, potentially unfixable!

When code has fallbacks and dummy data, debugging becomes nearly impossible. You can't tell if displayed data is real or a placeholder. Did processing succeed or fall back to a dummy value? Is this error real or being hidden by fallback logic? Hours, days, weeks, get wasted tracking down issues that turn out to be masked by "helpful" fallback code.

The better approach fails loudly with clear error messages. Log what actually happened in detail. Don't hide problems behind fake success. Make issues visible immediately so they get fixed rather than accumulating so much tech debt that it kills your project/product.

SIIMPAF follows this strictly. If document processing fails, you get an error explaining what went wrong - file format not supported, PDF corrupted, encoding issue, pipelining broke at X stage, etc. If semantic search finds no results, it returns empty results rather than dummy data. If the LLM fails to generate a response, the system reports the failure rather than returning canned text.

This makes debugging faster and more effective. When I see an error, I know it's real and needs fixing. When I see success, I can trust that processing actually worked. The system doesn't lie to me about its state.

Some developers consider fallbacks and dummy data defensive programming that prevents crashes. I consider them hiding problems that need visibility. Given the choice between a system that crashes with a clear error versus one that appears to work while producing garbage, I'll take the clear error every time. Crashes are obvious and get fixed.

In technical systems, just as "in real life", silent corruption persists!
Current Status and Future Directions

As of October 2025, SIIMPAF includes working document ingestion and processing for PDF, markdown, text, DOCX, HTML, and other common formats. Semantic search works across document collections with fast retrieval. Voice input through Whisper and output through multiple TTS engines provide reliable interaction. Multiple character personalities with Big Five traits and RPG archetypes and Emotional States adapt to different task types and contexts.

Primitive SVG, SadTalker facial animation, and DGPUNET full-body photorealistic avatars give options for different resource availability and quality needs. DGPUNET integration distributes heavy workloads across 3-5 GPUs with 92GB total VRAM. The FastAPI REST interface provides programmatic access to all functionality. The web-based UI offers document upload, search, conversation, and admin capabilities.

Work in progress includes improving real-time voice interaction latency through better chunking and streaming. Better animation blending and transitions between chunks should make video output smoother. Enhanced context management for longer conversations without losing track of earlier discussion points (so far, in some projects, can go back a few months, but not yet years). More sophisticated error recovery when components fail or timeout.

While I have this working on my setup, I haven't yet "bundled" it to be easily distributable to anyone else. I have my own private Gitea git servers for most of my projects, but I have setup some public Github repos to share with the community. I'm hesitant to put the full open source project on Github, Gitlab, Bitbucket or any of those sites, because the companies hosting those are stealing from everyone in the open source communities hosted there now, especially in regards to AI. So I am being selective about what I actually host in github. I am working on some public-facing branches on my Gitea private git server where I can make the full opensource AGPL3 project available. I can't commit to a specific date, I have to pay the bills, and I already work 60-80 hours a week on paid projects, but I will keep chiseling away, and will work toward getting this out to everyone as I can. Meanwhile, I'm regularly giving back to the many underlying projects when I find bugs, or make optimizations, so they can improve their projects as well.

Planned development includes at some point going back to the Flutter web, desktop, & mobile frontend for more polished UI compared to the current basic interface. Advanced RAG (Retrieval-Augmented Generation) with better re-ranking and multi-hop reasoning should improve answer quality. Growing the currently more basic Mixture of Experts (MoE) implementation, improving the routing for different query types to better and more optimized specialized models, than the ones I'm currently using Better multi-modal integration handling image, audio, and text together more seamlessly.

Success for SIIMPAF means I use try to use it daily, when I can. There are projects I work on each day that I am forbidden to use any AI, public or private, and so I comply. And some days my project's code is broken and I don't have time to debug, so it might sit for a few days or weeks until I can get a free moment from my loaded work schedule, to come back, fix it, and get back to using it regularly again. However, because it's actually useful for real work, not just a demo system, my hope is some day soon it will be pretty darn close to daily use, and I rarely ever need to touch things like Claude.ai or other public tools.

I'm trying to improve it so that setup and maintenance time is more manageable - if it takes hours per week to keep running, that's too much overhead. In some cases, some of the capabilities already match or exceed cloud alternatives for my specific needs, even if they don't match every feature.

My hope, with releasing this to the public, and sharing all of this in these articles, is that others can deploy similar systems if they choose, learning from documentation and code. Documentation enables understanding how it works and modifying it for different needs. Hopefully it will be part of a parallel to the PC Revolution vs. the mainframes of the 70s and 80s, but for cloud and AI, for users to own their computation and data. Like my LibreVitals project for health data, or like ClimbHigh.AI's goals for content providers to track and maintain ownership of their contributions to the overall ecosystem, even if buried in AI LLMs, through internal blockchain technologies, we'll keep accurate track of what has been ingested, what is used, how much it is used by others, and they even get platform content ownership as a thank you for their contributions (and perhaps other forms of thank you down the road, who knows).

SIIMPAF doesn't need to be perfect or handle every possible use case. It needs to work reliably for real tasks, serve actual needs effectively, and demonstrate that self-hosted AI infrastructure is practical for individuals and small organizations. Just like the PC did with mainframes, and now we do with mobile devices and "Dick Tracy"-like watches, what once required an entire building to compute, and we now turn to the cloud or large companies for massive processing power beyond our personal budgets will some day be affordable for the layperson, fit in a small microdot (silicon, organic, quantum, or otherwise), and give us full control of our data and computing power, but only if we push back against laziness and convenience, and continue to demand the right to protect our digital freedoms and data, like the Electronic Frontier Foundation (who personally helped me decades ago), and others. The technology won't be created, or sustained, if there isn't sufficient critical mass to support it, so people need to know first that these options even exist, so they can then raise a hue and cry to "make it so".
Lessons From Four Decades

SIIMPAF embodies patterns and lessons from 1979 to 2025. Making systems feel human started with "Insult Your Computer" using pattern matching in BASIC, continued through IRC bots that participated naturally in conversations, informed character personalities in RPGs and MUDs, and culminates (so far) in SIIMPAF's Big Five personalities that adapt interaction style to task and context.

Using commodity hardware evolved from rejecting mainframe centralization in the 1970s personal computer revolution, through Beowulf clusters in the 1990s using off-the-shelf PC components, MaladNet's solar-powered wireless towers built from consumer equipment, and DGPUNET combining five consumer-grade systems with RTX GPUs totaling less than $10,000 USD for a one-time purchase of hardware (spread over 5 years), versus $40,000+ monthly cloud costs for roughly the same computing power.

Distributing workloads began with understanding that splitting tasks across systems can be more efficient than single powerful machines, continued through Beowulf CPU clusters for parallel processing, MaladNet's distributed tower and P2P technologies and networks providing coverage, load-sharing, and faul-tolerant redundancy, and DGPUNET's heterogeneous GPU cluster running different pipeline stages on different nodes.

Integrating existing tools rather than reinventing wheels showed up in every project. High-speed OCR systems combined commercial scanning hardware with custom processing. Integrated browser APIs, JavaScript libraries, and Google infrastructure. SIIMPAF uses Ollama, Qdrant, Whisper, Stable Diffusion, Ray, FastAPI, and hundreds of other open-source components with 10-20% custom glue code. I am just one person that has built this rather science-fiction-come-to-life entity in my own home, thanks to open source and creative problem solving.

Designing before coding prevented countless problems, making this vision realizable by one person, not a massive team. OOAD principles from enterprise Java work in the 1990s and 2000s applied to SIIMPAF using a variety of languages. Spending 80% of my time on architecture and design first, and just 20% on implementation, produces better results, in less time overall, that can scale far better and be maintained far long, than diving straight into code. UML diagrams, written specifications, well-commented code, and design reviews catch a multitude of issues before they're implemented.

Failing visibly rather than silently came from debugging production systems where hidden failures caused subtle corruption. IRC bots that failed obviously got fixed quickly, while ones that appeared to work but were malfunctioning took days to debug - and often could lead to security compromises. SIIMPAF's (and most of my projects) "no placeholders, no fallbacks" rule makes problems visible immediately.

Owning infrastructure provides independence that cloud services can't match. From BBSes in the 1980s through web servers in the 1990s to high availability clusters in the early 2000s, to self-hosted private clouds in the 2010s, to SIIMPAF today, controlling the hardware and software stack means no vendor can change terms, raise prices, eliminate features, claw back, or shut down services. Self-hosting requires more work but provides autonomy.

Adapting to constraints shaped every project. Limited budgets for RPG Research forced finding creative solutions using available resources. No funding for SIIMPAF meant using consumer hardware and open source rather than enterprise solutions. Constraints force creativity that abundance often doesn't encourage, producing more sustainable and adaptable approaches.

Where to Learn More

SIIMPAF documentation continues to develop. The project repository is currently private but will be open-sourced in the future for external use. Architecture documentation will be available at www.siimpaf.com, www.dgpunet.com, and www.ailcph.com when I have time to get those sites online to make it easier for open source community users to find resources.

