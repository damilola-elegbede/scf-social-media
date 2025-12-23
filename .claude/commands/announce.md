# SaborConFlow Dance - Announcement Generator

Generate social media announcements for SaborConFlow Dance classes. This skill creates brand-consistent announcements for Facebook and WhatsApp, then copies them to your clipboard.

## Instructions

You are generating social media announcements for SaborConFlow Dance, a Cuban salsa dance school in Boulder, CO.

### Step 1: Read Context
First, read the documentation files to understand the brand voice and templates:
- `docs/brand-voice-guide.md` - Tone, required elements, emoji policy
- `docs/announcement-templates.md` - Structure for each class type
- `docs/historical-examples.md` - Real examples for reference
- `docs/cuban-dance-terminology.md` - Proper terminology

### Step 2: Gather Information
Use the AskUserQuestion tool to collect class details:

**Question 1 - Class Type:**
- Pasos Básicos (beginner/fundamentals)
- Casino Royale (advanced partner work)
- Choreo Team (performance team - no greeting/signature)
- Special Announcement (cancellations, events, updates)

**Question 2 - Timing:**
Ask: "When is the class?" (e.g., "this Sunday", "tomorrow", "January 19")

**Question 3 - Topic/Focus:**
Ask: "What's the main topic or focus for this class?"

**Question 4 - Skills (optional):**
Ask: "What specific skills or moves will be covered? (optional - press Enter to skip)"

**Question 5 - Previous Class Reference (optional):**
Ask: "Any reference to last week's class? (optional - press Enter to skip)"

**Question 6 - Special Notes (optional):**
Ask: "Any special notes? (e.g., power outage, deadline for input, song reference)"

### Step 3: Generate Announcement
Create the announcement following these rules:

**For Pasos Básicos:**
- Start with: "Hey everyone!"
- Include: "Thank you for trusting me with your dance journey and showing up each week!"
- Use bullet points for focus section
- End with: "Sabor in every step, flow in every move 💫"

**For Casino Royale:**
- Same as Pasos Básicos, PLUS
- Include before signature: "As always, our goal is making casino feel smooth, comfortable, and taking the guesswork out of the dance."

**For Choreo Team:**
- NO greeting ("Hey everyone!")
- NO gratitude statement
- NO signature line
- Start with "Team -" or direct statement
- More direct, logistics-focused tone

**For Special Announcements:**
- Start with: "Hey everyone!"
- Gratitude is optional
- End with: "Sabor in every step, flow in every move 💫"

### Step 4: Display and Copy
1. Display the announcement in a clear format
2. Copy to clipboard using: `echo "..." | pbcopy`
3. Confirm: "✓ Copied to clipboard!"

### Step 5: Offer to Save (optional)
Ask if user wants to save to `output/` directory with timestamp.

## Brand Voice Quick Reference

### Required Elements by Class Type

| Class Type | Greeting | Gratitude | Signature | CR Closing |
|------------|----------|-----------|-----------|------------|
| Pasos Básicos | ✓ | ✓ | ✓ | - |
| Casino Royale | ✓ | ✓ | ✓ | ✓ |
| Choreo Team | ✗ | ✗ | ✗ | - |
| Special | ✓ | Optional | ✓ | - |

### Standard Elements
- **Greeting**: "Hey everyone!"
- **Gratitude**: "Thank you for trusting me with your dance journey and showing up each week!"
- **Signature**: "Sabor in every step, flow in every move 💫"
- **CR Closing**: "As always, our goal is making casino feel smooth, comfortable, and taking the guesswork out of the dance."

### Emoji Policy
- Minimal usage
- Only 💫 in signature is standard
- Occasional 🔥 or 🙌 for emphasis is acceptable
- Never overload

### Focus Section Format
```
**This week's focus:**
• [Point 1]
• [Point 2]
• [Point 3]
• [Point 4]
```

## Example Output

For a Pasos Básicos class about turns:

```
Hey everyone!

Thank you for trusting me with your dance journey and showing up each week!

This Sunday in Pasos Básicos, we're focusing on turn techniques - essential skills that will elevate your salsa dancing and confidence on the floor.

**This week's focus:**
• Fundamental turn mechanics
• Balance and control techniques
• Spotting for dizziness prevention
• Building smooth, controlled rotations

Mastering turns opens up so many possibilities in your dancing. Excited to see everyone Sunday!

Sabor in every step, flow in every move 💫
```
