# Part 3: Motion Magic with Nova Reel 🎬
*Transform static stories into engaging video content*

## Lights, Camera, AI Action! (5 min)

### 🎯 Learning Objectives
- Master video prompt engineering
- Create compelling story sequences
- Design for different social platforms
- Build motion into your marketing

### 🎬 From Designer to Director
Your understanding of timing, pacing, and visual flow translates perfectly to video!

## 🔧 Bedrock Console Setup for Nova Reel (10 min)

### Prerequisites
- Ensure you have requested model access for Amazon Nova Reel
- If not, go to "Model access" in the left navigation and request access

### Step 1: Create S3 Bucket for Video Storage
Nova Reel requires an S3 bucket to store generated videos.

1. **Open a new browser tab** and go to: https://console.aws.amazon.com/s3/
2. **Click** "Create bucket"
3. **Configure your bucket:**
   - **Bucket name**: `nova-reel-workshop-[your-name]` (must be globally unique)
   - **AWS Region**: Same as your Bedrock region
   - **Object Ownership**: ACLs disabled (recommended)
   - **Block Public Access**: Keep all settings checked (enabled)
   - **Bucket Versioning**: Disable
   - **Encryption**: Use default (SSE-S3)
4. **Click** "Create bucket"
5. **Copy your bucket name** for later use

### Step 2: Navigate to Video Playground
1. **Return to Bedrock console**
2. **In the left sidebar**, expand "Playgrounds"
3. **Click** "Video" under Playgrounds
4. **You'll see** the video generation interface

### Step 3: Select Nova Reel Model
1. **In the model provider dropdown**, select "Amazon"
2. **In the model dropdown**, select "Amazon Nova Reel"
3. **Interface elements:**
   - Prompt input panel
   - S3 configuration section
   - Video settings panel
   - Generation status area

### Step 4: Configure S3 Output
1. **In S3 Output Location**:
   - Click "Browse S3"
   - Select your bucket: `nova-reel-workshop-[your-name]`
   - Or manually enter: `s3://nova-reel-workshop-[your-name]/`
2. **Output prefix** (optional): `workshop-videos/`

### Step 5: Configure Video Settings
1. **Duration**: 5 seconds (start small)
2. **Resolution**: 720p (balanced quality/speed)
3. **Frame Rate**: 24 fps (cinematic feel)
4. **Aspect Ratio**: 16:9 (standard) or 9:16 (vertical)

### Step 6: Test Your Setup
**Quick test prompt:**
1. **Type in the prompt input area:**
```
5-second video: Smooth zoom into a modern computer screen showing code transforming into a beautiful app interface, tech blue colors, professional style
```
2. **Click the "Run" button**
3. **Note:** Video generation takes 2-5 minutes. You'll see:
   - "Generation in progress" status
   - Progress indicator
   - Link to view in S3 when complete

### 💡 Pro Tips:
- Start with shorter durations (5-10 seconds)
- Open S3 in another tab to view completed videos
- Download videos locally for quick preview
- Keep prompts organized by project/campaign

## Video Prompting Fundamentals (10 min)

### The Video Prompt Formula

```
[Scene description] + [Camera movement] + [Duration] + [Transitions] + [Style] + [Pacing] + [Audio notes]
```

### Key Video Vocabulary

**Camera Movements:**
- Static/locked shot
- Slow zoom in/out
- Pan left/right
- Tilt up/down
- Tracking/dolly shot
- Orbital/arc shot

**Transition Types:**
- Cut
- Fade in/out
- Cross dissolve
- Wipe
- Morph transition
- Match cut

**Pacing Descriptors:**
- Fast-paced/energetic
- Slow and contemplative
- Building momentum
- Rhythmic cuts
- Smooth flow

## Project 1: Developer Transformation Story (25 min)

### Creating Your 15-Second Narrative Arc

**Storyboard Structure:**
```
0-5 sec: Problem (Struggle)
5-10 sec: Discovery (Solution)
10-15 sec: Result (Success)
```

### Scene 1: The Struggle (0-5 seconds)

**Prompt:**
```
5-second video: Stressed developer at cluttered desk typing frantically, 
multiple error messages popping up on screen, clock spinning fast in 
background showing passing time, quick cuts between coffee cups multiplying, 
frustration building, dramatic lighting with red warning colors, 
fast-paced editing, tension-building music
```

**Shot Breakdown:**
- 0-1s: Wide shot of cluttered workspace
- 1-2s: Close-up of error messages
- 2-3s: Developer's frustrated expression
- 3-4s: Clock spinning, papers piling up
- 4-5s: Head in hands moment

### Scene 2: The Discovery (5-10 seconds)

**Prompt:**
```
5-second video: Developer discovers AI assistant, magical moment as 
AI interface appears with gentle glow, workspace begins transforming, 
clutter dissolving, screens showing success, color shift from red to 
blue/purple, hopeful music swelling, smooth camera push-in, 
particle effects suggesting transformation
```

**Shot Breakdown:**
- 5-6s: AI icon appears with sparkle effect
- 6-7s: Interface elegantly sliding in
- 7-8s: Code writing itself
- 8-9s: Errors resolving to checkmarks
- 9-10s: Developer's expression changing to wonder

### Scene 3: The Success (10-15 seconds)

**Prompt:**
```
5-second video: Happy developer in bright, organized workspace, 
smooth workflow visualization, coffee enjoyed leisurely, 
plants and natural light, graphs showing productivity increase, 
team celebrating in background, warm color palette, uplifting music, 
slow motion high-five, ending with company logo reveal
```

**Shot Breakdown:**
- 10-11s: Clean workspace reveal
- 11-12s: Smooth workflow visualization
- 12-13s: Team celebration moment
- 13-14s: Success metrics animation
- 14-15s: Logo with tagline

### 🎯 Platform-Specific Variations

**Instagram Reel (9:16 vertical):**
- Tighter framing
- Text overlays for sound-off viewing
- Hook in first 1 second
- Loop-friendly ending

**LinkedIn Video (16:9 or square):**
- Professional tone
- Include captions
- Data visualization focus
- Thought leadership angle

**TikTok (9:16 vertical):**
- Trending audio consideration
- Faster pacing
- Relatable moments
- Strong hook

## Project 2: Product Feature Highlights (20 min)

### Kinetic Typography for Key Benefits

**Speed Benefit Video:**
```
7-second kinetic typography video: Words "SLOW" morphing into "FAST", 
"HOURS" shrinking to "MINUTES", "DEPLOY MONTHLY" transforming to 
"DEPLOY DAILY", dynamic motion graphics, tech-inspired particle effects, 
electric blue color scheme, rhythmic animations synced to upbeat music
```

### Feature Showcase Reel

**Multi-Feature Prompt:**
```
10-second feature montage: Split screen showing 4 key features 
simultaneously - AI code completion, automated testing, instant deployment, 
real-time collaboration. Each quarter animates in sequence, clean 
minimal design, smooth transitions, professional tech aesthetic
```

### Before/After Comparison

**Split-Screen Demo:**
```
8-second split-screen comparison video: Left side showing traditional 
coding (slow, manual, errors), right side showing AI-assisted coding 
(fast, automated, success), synchronized actions highlighting speed 
difference, progress bars racing, modern versus outdated visual styling
```

## Project 3: Social Media Snippets (15 min)

### Instagram Reel: "Day in the Life"

```
15-second vertical video: Developer's day with AI assistant, 
time-lapse style, morning coffee to evening success, 
5 quick scenes showing progression, trendy transitions, 
upbeat music, captions highlighting time saved, 
ending with call-to-action
```

### LinkedIn Thought Leadership

```
20-second professional video: Executive discussing AI transformation, 
minimal kinetic text highlighting key stats (50% faster, 
3x more features, 90% satisfaction), clean corporate background, 
subtle animations, authoritative yet approachable tone
```

### Twitter/X Teaser

```
6-second loop video: Mesmerizing visualization of code writing itself, 
AI particles flowing into perfect functions, seamless loop point, 
eye-catching for timeline scroll-stopping, minimal text overlay
```

## Advanced Video Techniques (10 min)

### 1. Seamless Loops
```
Create perfect loop: End frame matches start frame, continuous motion, 
hypnotic effect for extended viewing, suitable for background video
```

### 2. Match Cut Mastery
```
Transition between scenes using matching: shapes, movements, colors, 
or objects. Creates smooth visual flow and professional editing feel
```

### 3. Speed Ramping
```
Variable speed video: Start slow motion for emphasis, speed up for 
energy, return to normal for resolution, creates dynamic viewing experience
```

### 4. Text Animation Styles
- **Typewriter:** Classic coding feel
- **Particle burst:** Tech innovation
- **Smooth morph:** Transformation story
- **Glitch effect:** Problem to solution

## 🏆 Rapid Video Challenge (10 min)

Create these video concepts:
1. 5-second product logo animation
2. 10-second customer testimonial template
3. 15-second event promotion
4. 6-second loading animation
5. 8-second error-to-success story
6. 12-second team culture video
7. 7-second feature comparison
8. 20-second product demo
9. 3-second CTA animation
10. Perfect loop background video

## Platform Optimization Guide 📱

### Video Specifications Cheat Sheet

**Instagram Feed:** 1:1, up to 60 seconds
**Instagram Reels:** 9:16, up to 90 seconds
**Instagram Stories:** 9:16, up to 60 seconds
**TikTok:** 9:16, up to 10 minutes
**LinkedIn:** 16:9 or 1:1, up to 10 minutes
**Twitter/X:** 16:9, up to 2:20
**YouTube Shorts:** 9:16, up to 60 seconds

### Engagement Optimization

**First 3 Seconds Matter:**
- Hook with unexpected visual
- Ask intriguing question
- Show dramatic transformation
- Use pattern interrupt

**Sound-Off Strategy:**
- Always include captions
- Visual storytelling priority
- Clear text overlays
- Expressive visuals

## Your Video Prompt Toolkit 🎬

### Basic Video Template:
```
[Duration] video: [Scene description], [Camera movement], 
[Visual style], [Color palette], [Transitions], [Pacing], 
[Music/audio notes], [Platform specifications]
```

### Quick Video Styles:

**Tech Demo:**
```
...screen recording style, smooth cursor movements, highlight 
interactions, clean UI, professional pace, subtle sound effects
```

**Lifestyle Marketing:**
```
...real-world setting, natural movements, authentic moments, 
warm lighting, lifestyle photography in motion, ambient sound
```

**Motion Graphics:**
```
...abstract animations, geometric shapes, smooth morphing, 
brand colors, rhythmic movement, electronic music sync
```

## ✅ Pre-Campaign Checklist

You should now have:
- [ ] 15-second story video concept
- [ ] Platform-specific variations
- [ ] Feature highlight videos
- [ ] Social media snippets
- [ ] Looping background video
- [ ] Your video prompt templates

## 🚀 Ready for the Grand Finale?

Time to combine everything into a cohesive campaign!

---

### 💭 Quick Reflection
*What video format excited you most? Which platform will you target first?*