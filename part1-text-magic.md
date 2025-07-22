# Part 1: Text Magic with Nova Pro 📝
*Transform your copywriting with AI-powered creativity*

## Welcome to the World of AI Copywriting! (10 min)

### 🎯 Learning Objectives
- Master prompt engineering for marketing copy
- Create multiple variations quickly
- Develop your unique AI + human creative process

### 🤝 Icebreaker Activity
**"Worst Marketing Copy Hall of Shame"**
Share the most cringe-worthy marketing copy you've encountered. We'll use AI to fix it!

## 🔧 Bedrock Console Setup for Nova Pro (5 min)

### Prerequisites
- Ensure you have requested model access for Amazon Nova Pro
- If not, go to "Model access" in the left navigation and request access

### Step 1: Access AWS Console
1. **Open your browser** and go to: https://console.aws.amazon.com
2. **Sign in** with your AWS credentials
3. **Check your region** (top-right corner) - ensure US East (N. Virginia) is selected

### Step 2: Navigate to Bedrock
1. **In the search bar**, type "Bedrock"
2. **Click** "Amazon Bedrock" from the results
3. You'll land on the Bedrock dashboard

### Step 3: Access Nova Pro for Text, Nova Canvas for Images, Nova Reels for Video
1. **In the left sidebar**, expand "Test"
2. **Click** "Text" under Test
3. **From the model provider dropdown**, select "Amazon"
4. **From the model dropdown**, choose "Amazon Nova Pro", "Amazon Nova Canvas" and "Amazon Nova Reels".
5. You should see:
   - Model selector showing "Amazon Nova Pro", "Amazon Nova Pro", "Amazon Nova Canvas" and "Amazon Nova Reels".
   - Prompt input panel for your text
   - Configuration settings on the right
   - Generated output area below

### Step 4: Configure Settings
1. **Temperature**: Set to 0.7 (good balance of creativity/consistency)
2. **Max tokens**: 500 (sufficient for most marketing copy)
3. **Top P**: Leave at default (0.9)
4. **Stop sequences**: Leave empty for now

### Step 5: Test Your Setup
**Quick test prompt:**
1. **Type in the prompt input area:**
```
Write a 5-word tagline for a coffee shop
```
2. **Click the "Run" button**
3. **Expected response:** You should see a creative tagline appear in the generated output area

### 💡 Pro Tips:
- Keep this tab open throughout Part 1
- Use the "Clear" button between prompts to reset the conversation
- Copy successful prompts to your notes
- Use the copy icon to save generated responses
- The "Run" button executes your prompt

## Understanding Nova Pro Prompts (10 min)

### The Anatomy of a Great Prompt

```
[Task] + [Context] + [Audience] + [Tone] + [Constraints]
```

**Example:**
```
Task: Write a tagline
Context: for a developer productivity tool
Audience: targeting senior developers
Tone: professional yet approachable
Constraints: under 10 words
```

### 🎨 The Designer's Advantage
As designers, you already think in:
- Brand voice
- Target personas
- Emotional impact
- Visual hierarchy

Apply these same principles to text!

## Exercise 1: The Happy Developer Story (15 min)

### Round 1: Basic Prompt
Try this first:
```
Write a tagline about a developer using new tools
```

**What you'll likely get:** Generic, uninspiring copy

### Round 2: Enhanced Prompt
Now try:
```
Create a punchy tagline for a tech startup showing a developer 
who switched from manual coding to automated development. 
Emphasize time saved (50%) and creative freedom gained. 
Make it memorable and under 8 words. Avoid technical jargon.
```

### Round 3: Your Turn!
Create taglines for these scenarios:
1. Developer discovering automation for the first time
2. Team celebrating faster deployment
3. Company showcasing productivity gains

### 💡 Pro Tip: The "Before/After" Formula
This powerful formula creates instant narrative tension and resolution - perfect for headlines, social posts, and email subject lines. It works because it acknowledges the reader's current pain while promising a better future.

**Formula Templates:**
```
"From [pain point] to [solution] in [timeframe]"
"No more [problem]. Hello [benefit]."
"[Old way] is out. [New way] is in."
```

**Real Examples:**
- "From 8-hour deploys to 8-minute releases in 30 days"
- "No more debugging nightmares. Hello cleaner code."
- "Manual testing is out. Automated confidence is in."

**Why It Works:**
1. **Relatability**: Acknowledges current struggles
2. **Hope**: Promises transformation
3. **Clarity**: Simple, memorable structure
4. **Action**: Implies movement and progress

**Try It Yourself:**
When prompting Nova Pro, use this structure:
```
Create a headline using the before/after formula showing how developers 
go from [specific pain point] to [specific benefit].
Make it punchy and under 10 words.
```

## Exercise 2: Marketing Copy Variations (20 min)

### The Multiplication Method
One concept → Multiple formats

**Your Mission:** Take the concept "Modern tools make developers happier and more productive"

Create 5 variations of each:

### 1. Social Media Posts

**Platform-Specific Writing Strategies**

Each social platform has unique audience expectations and content formats. Understanding these differences is crucial for engagement.

**LinkedIn (Professional Storytelling)**
```
Prompt: Write a LinkedIn post about developers using modern tools to boost 
productivity. Include a surprising statistic, personal insight, 
and call-to-action. Professional tone, 100-150 words.
```

**Why This Prompt Works:**
- **Statistic**: Builds credibility and stops the scroll
- **Personal insight**: Creates connection and authenticity
- **CTA**: Drives meaningful engagement
- **Word count**: Optimal for LinkedIn's algorithm

**Example Output Structure:**
```
Hook: Surprising stat or bold statement
Story: Personal experience or observation
Insight: What this means for the industry
CTA: Question or invitation to share
```

**Twitter/X (Conversation Starters)**
```
Prompt: Create a tweet thread (3 tweets) about developer happiness 
with modern tools. Make it conversational, include emojis, and end 
with a question to drive engagement.
```

**Thread Strategy:**
- Tweet 1: Hook with bold claim or question
- Tweet 2: Supporting evidence or example
- Tweet 3: Open-ended question for replies

**Engagement Tactics:**
- Emojis for visual breaks 🚀
- Short sentences for readability
- Questions that invite personal experiences

**Instagram (Visual Storytelling)**
```
Prompt: Write Instagram caption for image of happy developer. 
Start with attention-grabbing first line. Include 3-5 relevant 
hashtags. Inspirational but authentic tone.
```

**Instagram Formula:**
1. **Hook** (first line): Must work as preview text
2. **Story** (2-3 lines): Quick, relatable narrative
3. **Inspiration** (1-2 lines): Uplifting message
4. **CTA**: Simple action (double-tap, share, comment)
5. **Hashtags**: Mix of broad (#coding) and niche (#AIforDevs)

### 2. Email Subject Lines

**The Science of Subject Lines**
Your subject line determines whether your email gets opened. Different psychological triggers work for different audiences and contexts.

**Psychological Triggers Explained:**

**Curiosity Gap** 
- Example: "The secret tool your dev team isn't using (yet)"
- Why it works: Creates knowledge gap that begs to be filled
- Best for: Awareness stage, new audiences

**FOMO (Fear of Missing Out)**
- Example: "Why 73% of developers already switched to AI"
- Why it works: Social proof + urgency
- Best for: Consideration stage, competitive markets

**Direct Benefit**
- Example: "Ship features 2x faster starting today"
- Why it works: Clear value proposition
- Best for: Decision stage, practical audiences

**Provocative Question**
- Example: "Still coding everything manually?"
- Why it works: Challenges status quo
- Best for: Problem-aware audiences

**Personalization**
- Example: "[Name], your team could save 20 hours/week"
- Why it works: Individual relevance + specific benefit
- Best for: Warm leads, existing relationships

**Nova Pro Subject Line Generator:**
```
Create 5 email subject lines for a developer productivity tool launch.
Mix psychological approaches: curiosity, FOMO, direct benefit,
question, and personalization. Keep under 50 characters.
Include one with a specific metric or timeframe.
Target: Engineering managers at mid-size companies.
```

### 3. Call-to-Action Buttons

**Moving Beyond Generic CTAs**
Great CTAs combine action verbs with specific benefits. They should create urgency while clearly communicating value.

**Effective CTA Examples:**
- "Start Creating Faster →" (Action + Benefit + Direction)
- "See AI in Action" (Curiosity + Demonstration)
- "Join Happy Developers" (Community + Emotional Appeal)
- "Get Your Time Back" (Personal Benefit + Value)
- "Transform Your Workflow" (Change + Professional Impact)

**CTA Psychology:**
- **Action Verbs**: Start, See, Join, Get, Transform
- **Benefit Focus**: Faster, Happy, Time Back
- **Visual Cues**: Arrows (→) suggest movement
- **Emotional Triggers**: FOMO, belonging, improvement

**Nova Pro Prompt for CTAs:**
```
Generate 5 call-to-action button texts for a developer tool.
Each should be 2-4 words, start with an action verb, and imply
a specific benefit. Avoid generic phrases like "Learn More" or "Click Here".
Target audience: Senior developers who value efficiency.
```

**Pro Tip**: Test CTAs in pairs - one emotional ("Join the Revolution") vs one logical ("Reduce Deploy Time")

### 🎯 A/B Testing Mindset

**Why Multiple Variations Matter**
Never settle for your first idea. Creating variations lets you test what resonates with your specific audience.

**Testing Dimensions:**

**Emotional vs. Logical Appeals**
- Emotional: "Join thousands of happy developers"
- Logical: "Reduce deployment time by 67%"
- Test with: Different audience segments

**Short vs. Long Copy**
- Short: "Code faster. Ship sooner."
- Long: "Transform your development workflow with tools that understand your code"
- Test for: Platform and placement

**Feature vs. Benefit Focus**
- Feature: "Advanced code completion"
- Benefit: "Finish projects weeks earlier"
- Test when: Audience familiarity varies

**Urgent vs. Evergreen Messaging**
- Urgent: "Limited beta access ending soon"
- Evergreen: "The future of coding is here"
- Test based on: Campaign goals

**Nova Pro Variation Generator:**
```
Create 4 versions of this message: "Modern tools help developers code faster"
Version 1: Emotional appeal, short
Version 2: Logical/data-driven, short  
Version 3: Feature-focused, medium length
Version 4: Benefit-focused with urgency
Keep consistent core message, vary approach.
```

## Advanced Techniques (10 min)

### 1. Brand Voice Injection

**Channeling Established Brand Personalities**
Learn from successful brands by adapting their voice patterns to your message. This technique helps you quickly achieve different tones.

```
Prompt: Rewrite this tagline in the style of [brand]:
- Apple: Minimalist, revolutionary
- Nike: Motivational, action-oriented  
- Slack: Friendly, conversational
Do not mention products or brands.
```

**Brand Voice Characteristics:**

**Apple Style:**
- Fewer words, bigger impact
- Focus on the experience, not features
- Example: "Code. Reimagined."

**Nike Style:**
- Empowering, challenge-oriented
- Action verbs and achievement
- Example: "Just Ship It"

**Slack Style:**
- Approachable, slightly playful
- Like talking to a helpful colleague
- Example: "Coding, but make it fun"

### 2. Emotional Targeting

**Connecting Through Specific Emotions**
Different emotions drive different actions. Choose the emotion that matches your campaign goal.

```
Create copy that evokes [emotion]:
- Relief: "Finally, coding without the headaches"
- Excitement: "Unleash your creative potential"
- Confidence: "Build like you've always imagined"
```

**Emotion-Action Mapping:**
- **Relief** → Problem-solving products
- **Excitement** → New features/launches
- **Confidence** → Enterprise/professional tools
- **Joy** → Team/culture initiatives
- **Pride** → Achievement/success stories

**Nova Pro Emotional Prompt:**
```
Write 3 taglines for a developer productivity tool, each evoking a different emotion:
1. Relief (solving a pain point)
2. Excitement (discovering possibilities)
3. Confidence (mastering the tool)
Target: Developers who feel overwhelmed by complexity
```

### 3. Constraint Creativity

**Why Constraints Spark Innovation**
Limitations force creative solutions. Use constraints to break out of generic patterns.

```
Write this message with constraints:
- Only 5 words
- No adjectives
- As a haiku
- Using only questions
```

**Creative Constraint Exercises:**

**Word Limit Challenge:**
- 5 words: Forces absolute clarity
- Example: "Ship faster. Sleep better. Repeat."

**Grammar Restrictions:**
- No adjectives: Focus on strong nouns/verbs
- Example: "Code writes itself. Developers create."

**Format Experiments:**
- Haiku: Adds rhythm and memorability
- Example: "Errors fade away / Smart tools guide your path / Success blooms at last"

**Question-Only Copy:**
- Engages reader's curiosity
- Example: "What if coding was easy? What if bugs fixed themselves? What if you could focus on creating?"

## 🏆 Mini Challenge: Speed Round!

**5 minutes, 10 pieces of copy:**
1. Hero headline
2. Subheadline
3. Feature benefit
4. Customer testimonial
5. FAQ answer
6. Error message
7. Success notification
8. Onboarding welcome
9. Upgrade prompt
10. Thank you message

**Theme:** Happy developer using modern tools

## Key Takeaways & Your Prompt Toolkit

### 🎨 Remember:
- Specific prompts = Better results
- Iterate and refine
- Mix AI efficiency with human creativity
- Always consider your audience

### 📋 Your Starter Prompt Templates:

**For Headlines:**
```
Create a [length] headline for [product/service] that 
appeals to [audience] by highlighting [key benefit]. 
Use [tone] language and avoid [what to avoid].
```

**For Social Posts:**
```
Write a [platform] post about [topic] for [audience]. 
Include [specific elements]. Make it [tone] and around 
[length]. End with [call-to-action type].
```

**For Email Copy:**
```
Draft a [type] email for [campaign goal]. Target [persona] 
who struggles with [pain point]. Highlight [solution] and 
include [number] benefit points. Subject line should create 
[emotion/curiosity].
```

## ✅ Checkpoint

Before moving to Part 2, you should have:
- [ ] Created at least 15 pieces of copy
- [ ] Tried 3 different prompt styles
- [ ] Found your favorite prompt formula
- [ ] Saved your best outputs

## 🚀 Next Up: Visual Storytelling!

Ready to bring these words to life with images? Let's dive into Nova Canvas!

---

### 💬 Quick Reflection
*What surprised you most about AI copywriting? Share with your workshop partner!*
