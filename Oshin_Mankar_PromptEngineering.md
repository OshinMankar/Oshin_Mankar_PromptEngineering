# Prompt Engineering Portfolio
Name: Oshin Mankar

Date: 02/06/2026

LLM Used: Claude 

## Part 1: Prompt Design & Iteration
### 1.1 Scenario A: Technical Explanation

**Goal:** Explain "What is cloud computing" to a 10-year-old.

**V1 - Initial Prompt:**

> "Explain Cloud Computing"

Cloud computing refers to the delivery of computing services — including servers, storage, databases, networking, software, and analytics — over the internet ("the cloud") to offer faster innovation, flexible resources, and economies of scale. Instead of owning and maintaining physical data centers or servers, organizations can access technology services on an as-needed basis from a cloud provider such as Amazon Web Services, Microsoft Azure, or Google Cloud. Users typically pay only for the cloud services they use, helping them reduce operating costs and scale as their business needs change.

**V2 - Refined Prompt:**

> "As a friendly teacher, explain cloud computing to a 10-year-old using a simple analogy"

**V2 Output:**

You know how you don't keep all your favourite movies stored on a single DVD at home anymore — instead you just open Netflix and they're all there? Cloud computing is a bit like that, but for any kind of file or program. Instead of saving everything on your own computer, you save it on a giant computer somewhere else (called a server), and you can reach it from anywhere as long as you have the internet. Big companies use this so they don't have to buy millions of computers — they just rent space on someone else's giant computer instead.

**V3 - Final Prompt:**

> "You are a friendly primary school teacher explaining technology to curious 10-year-olds. Explain what cloud computing is using a relatable, fun analogy from everyday life that a child would immediately understand. Avoid all technical jargon. Keep the explanation under 100 words and end with one fun fact that will surprise them."

**V3 Output:**

Imagine if instead of keeping your drawings in a folder at home, you kept them all in a magic library in the sky — and you could walk into any library branch anywhere in the world and find your exact drawings waiting for you. Cloud computing is just like that magic library, but for computer files, photos, videos, and apps! Companies like Google and Amazon own giant buildings full of computers that store everyone's stuff safely. You can reach your things from any device, anywhere.

*Fun fact: If you've ever used Google Drive or iCloud, you've already used the cloud!*

**Iteration table:**

| Version |	Prompt | What Changed |	Why This Improved the Output |
|---------|--------|--------------|-------------------------------|
| V1 | Explain Cloud Computing | N/A | N/A |
| V2 | As a friendly teacher, explain cloud computing to a 10-year-old using a simple analogy	| Added role, target audience, and analogy instruction |	Specifying a 10-year-old audience forced the model away from corporate language like "economies of scale"; the analogy instruction produced the Netflix comparison which is immediately relatable |
| V3	| Added "primary school teacher" role detail, "fun" tone, 100-word limit, no-jargon rule, and fun fact requirement	| Added format constraints, stronger role framing, and surprise element |	The word limit prevented over-explanation; asking for something "surprising" pushed the model to end with a real-world connection (Google Drive/iCloud) that makes the concept click personally for the reader |

### 1.1 Scenario B: Professional Email

**Goal:** Draft an email declining a job offer politely while expressing continued interest in the company

**V1 - Initial Prompt:**

> "Write an email declining a job offer."

**V1 - Output:**

Subject: Job Offer — Decision

Dear Hiring Manager,

Thank you for offering me the position. After careful consideration, I have decided to decline the offer. I appreciate the opportunity and wish the company success.

Regards,
[Name]

**V2 - Refined Prompt:**

> "You are a professional career coach helping a candidate write a polished email. The candidate is declining a job offer from ROI Magnet for a Software Engineer role. The reason is that they have accepted a position elsewhere that better matches their current career goals. The tone should be warm, professional, and show interest in future opportunities."

**V2 - Output:**

Subject: Re: Software Engineer Offer — TechNova Solutions

Dear [Hiring Manager's Name],

Thank you so much for offering me the Software Engineer position at ROI Magnet. I genuinely enjoyed learning about the team and the exciting work you are doing in the industry.

After much reflection, I have decided to accept another opportunity that aligns more closely with my immediate career goals. This was not an easy decision, as TechNova impressed me throughout the process.

I have a great deal of respect for your team and would love to stay in touch. I hope our paths cross again in the future.

Warm regards,
[Your Name]

**V3 Final Prompt:**

> "You are a professional career coach helping a job candidate write an email declining a job offer. Details- the company is ROI Magnet, the role is Junior Data Analyst, and the candidate is declining because they accepted a competing offer at a startup that better fits their passion for machine learning. The email should- open with sincere gratitude, give a brief and honest reason without oversharing, compliment the team or company specifically, and close with a genuine invitation to stay connected. Tone: warm, professional, and memorable. Length: 150–200 words."

**V3 Output:**

Subject: Junior Data Analyst Offer — Grateful Decision

Dear [Hiring Manager's Name],

Thank you sincerely for offering me the Junior Data Analyst role at TechNova Solutions. It was a privilege to meet your team and learn about the impactful analytics work you are building.

After careful reflection, I have decided to accept another offer at an early-stage machine learning startup that closely matches the direction I want to grow in professionally. This was genuinely one of the hardest decisions I have made — TechNova's collaborative culture and the clarity of your product vision stood out to me throughout the entire process.

I have tremendous respect for what your team is doing, and I hope to stay connected. Please do not hesitate to reach out — I would welcome the chance to cross paths again as we both move forward.

Thank you once more for your time and generosity throughout this process.

Warm regards,
[Your Name]

**Iteration table:**

| Version |	Prompt | What Changed |	Why This Improved the Output |
|---------|--------|--------------|-------------------------------|
| V1 | Write an email declining a job offer | N/A | N/A |
| V2 | Added role (career coach), company name, role title, reason for declining, and desired tone | Introduced role, context, and tone guidance | Gave the model enough context to write something genuinely warm rather than a generic two-line decline; the specific company name made the output feel personal |
| V3	| Added structural requirements (4 numbered goals), word count constraint, and emotional angle (passion for ML) | Added output structure and emotional specificity | Structuring the email's four required beats ensured completeness; word count prevented rambling; the ML detail made the reason sound authentic rather than vague |

### 1.1 Scenario C: Creative content

**Goal:** Generate a creative marketing tagline for a new eco-friendly water bottle brand - Aqualoop"

**V1 — Initial Prompt:**

> "Write a marketing tagline for an eco-friendly water bottle."

**V1 Output:**

- "Stay hydrated, save the planet."
- "Drink well. Live green."
- "Eco-friendly hydration for a better tomorrow."

**V2 — Refined Prompt:**

> "You are a professional copywriter. Write 5 punchy marketing taglines for Aqualoop, an eco-friendly water bottle brand targeting environmentally conscious millennials aged 25–35. The taglines should feel fresh and modern, not clichéd."

**V2 Output:**

- "Refill the world, one sip at a time."
- "Because the ocean doesn't need more plastic."
- "Good for you. Better for the planet."
- "Drink today. Protect tomorrow."
- "Your thirst. Our mission."

**V3 — Final Prompt:**

> "You are an award-winning brand copywriter specializing in sustainability and lifestyle brands. Write 3 tagline options for Aqualoop, a premium eco-friendly water bottle brand targeting environmentally conscious consumers aged 22–35 who see sustainability as part of their identity, not just a choice. Each tagline should be- under 7 words, emotionally resonant, and memorable. After each tagline, write one sentence explaining the emotional angle it targets."

**V3 Output:**

**Option 1: "Loop it. Lose nothing."**
*This tagline uses the brand name cleverly and appeals to the audience's desire for a zero-waste lifestyle where choosing sustainability means giving nothing up.*

**Option 2: "Carry less. Leave more."**
*Targets the minimalist, low-impact identity of the audience — the idea that a lighter footprint is something to be proud of.*

**Option 3: "Every sip. Every choice. Aqualoop."**
*Creates a sense of daily ritual and intentionality, positioning the bottle as a quiet symbol of values the customer lives by.*

**Iteration table:**

| Version |	Prompt | What Changed |	Why This Improved the Output |
|---------|--------|--------------|-------------------------------|
| V1 | Write a marketing tagline for an eco-friendly water bottle. | N/A | N/A |
| V2 | Added role (copywriter), brand name, target audience, and instruction to avoid clichés | Introduced role, brand name, and audience | Specifying the audience and the "no clichés" constraint pushed the model away from generic sustainability phrases toward more specific and modern language |
| V3 | Added premium brand positioning, identity-based audience description, word limit per tagline, and request for rationale | Added emotional brief and structural constraints | Asking the model to explain each tagline's emotional angle forced it to think like a strategist, not just a wordsmith — resulting in taglines with distinct and intentional emotional targets |

### 1.3 Role and Context Analysis

Adding role assignment and context dramatically improved the quality of outputs in both Scenarios B and C. In Scenario B, framing the task as advice from a "professional career coach" prompted the model to produce language that felt genuinely warm and relationship-aware, rather than the cold, transactional tone it defaulted to with a bare prompt. In Scenario C, assigning the role of "award-winning brand copywriter specializing in sustainability" shifted the model from producing generic eco-slogans to crafting taglines with a distinct strategic angle, because the role itself implied a higher standard of craft. Providing context, such as the specific company name, target audience demographics, and the emotional identity of the consumer, gave the model the raw material it needed to personalize the output rather than produce something that could have been written for any brand. Without role and context, the model essentially guesses what the requester wants; with them, it has a clear brief to write against, which is exactly how professional writing actually works.

## Part 2: Temperature & Parameter Control

### 2.1 Temperature Experimentation

**Task chosen:** Writing a product description for a laptop (the "NovaPro 15").

**Prompt used (identical across all three runs):**

> "Write a 3–4 sentence product description for the NovaPro 15, a mid-range laptop with a 15.6-inch display, Intel Core i5 processor, 16GB RAM, and 512GB SSD."

**Low Temperature (0.1)**
*Simulated by appending: "Be precise and consistent. Stick to the specifications."*

**Output:**

The NovaPro 15 features a 15.6-inch display, an Intel Core i5 processor, 16GB of RAM, and a 512GB SSD. It is designed for everyday computing tasks including document editing, web browsing, and light multitasking. The system offers reliable performance in a standard mid-range form factor. It is suitable for students and office professionals who require a dependable machine.

**Medium Temperature (0.7)**
*Prompt used as-is.*

**Output:**

Meet the NovaPro 15 — a powerful yet approachable laptop built for people who get things done. Powered by an Intel Core i5 processor with 16GB of RAM and a speedy 512GB SSD, it handles everything from spreadsheets to creative projects without breaking a sweat. The generous 15.6-inch display gives you the screen real estate to work, stream, and create in comfort. Whether you're a student, a remote worker, or someone who just wants a reliable machine that keeps up with life, the NovaPro 15 delivers.

**High Temperature (1.3)**
*Simulated by appending: "Be creative and explore diverse, imaginative ideas."*

**Output:**

The NovaPro 15 isn't just a laptop — it's a quiet co-conspirator in whatever you're building, writing, or dreaming up next. Beneath its understated chassis lives an Intel Core i5 that chews through to-do lists and side projects alike, backed by 16GB of RAM that keeps every tab, track, and thought alive at once. The 512GB SSD loads your world in seconds, and the sweeping 15.6-inch display makes sure none of it goes to waste. Think of it as the kind of dependable companion that never shows off but never lets you down.

**Comparison Table:**

| Aspect | Low (0.1) | Medium (0.7) | High (1.3) |
|--------|-----------|--------------|------------|
| Tone | Dry, clinical, factual | Friendly, conversational, enthusiastic | Poetic, metaphorical, personality-driven |
| Creativity | Very low — spec recitation | Moderate — adds appeal without sacrificing clarity | High — uses metaphor and imagery |
| Factual accuracy | Highest — no embellishment | High — accurate with added readability | Moderate — accurate but secondary to voice |
| Word choice | Plain, technical | Natural, accessible | Expressive, literary |
| Best use case | Technical data sheets, spec pages | General product pages, e-commerce listings | Brand campaigns, lifestyle marketing |

### 2.2 Analysis & Recommendations

Low temperature is best suited for tasks where consistency and factual precision are non-negotiable, such as generating medical or legal summaries, writing technical documentation, or producing structured data outputs like JSON or code, any context where a surprising or inventive response would be a problem rather than an asset. High temperature works well for creative tasks where originality is the goal, such as brainstorming brand concepts, writing poetic or narrative copy, generating diverse story openings, or ideating across many different angles for a marketing campaign where you want unexpected directions. For this product description task, medium temperature produced the best result- it retained all the accurate technical specifications while adding the kind of human, readable voice that actually makes someone want to buy a laptop, the low temperature output felt too dry to be persuasive, and the high temperature output, while entertaining, prioritized metaphor over information in a way that might frustrate a shopper looking for facts. This experiment reinforced that temperature is not about "better or worse" but about matching the model's randomness to the purpose of the task — and that most practical writing tasks live in the medium range.















