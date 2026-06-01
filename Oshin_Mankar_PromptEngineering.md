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

> "You are a professional career coach helping a candidate write a polished email. The candidate is declining a job offer from TechNova Solutions for a Software Engineer role. The reason is that they have accepted a position elsewhere that better matches their current career goals. The tone should be warm, professional, and leave the door open for future opportunities."

**V2 - Output:**

Subject: Re: Software Engineer Offer — TechNova Solutions

Dear [Hiring Manager's Name],

Thank you so much for offering me the Software Engineer position at TechNova Solutions. I genuinely enjoyed learning about the team and the exciting work you are doing in the industry.

After much reflection, I have decided to accept another opportunity that aligns more closely with my immediate career goals. This was not an easy decision, as TechNova impressed me throughout the process.

I have a great deal of respect for your team and would love to stay in touch. I hope our paths cross again in the future.

Warm regards,
[Your Name]

**V3 Final Prompt:**

> "You are a professional career coach helping a job candidate write a gracious email declining a job offer. Details: the company is TechNova Solutions, the role is Junior Data Analyst, and the candidate is declining because they accepted a competing offer at a startup that better fits their passion for machine learning. The email should: (1) open with sincere gratitude, (2) give a brief and honest reason without oversharing, (3) compliment the team or company specifically, and (4) close with a genuine invitation to stay connected. Tone: warm, professional, and memorable. Length: 150–200 words."





































