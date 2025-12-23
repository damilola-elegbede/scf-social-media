# SaborConFlow Social Media

Automated announcement generator for SaborConFlow Dance - a Cuban salsa dance school in Boulder, CO.

## Quick Start

From this directory in Claude Code:

```
/announce
```

Claude will interactively ask for class details and generate a brand-consistent announcement, then copy it to your clipboard automatically.

## How It Works

1. Run `/announce` in Claude Code
2. Answer questions about the class (type, date, topic, skills)
3. Receive a formatted announcement
4. Announcement is automatically copied to clipboard
5. Paste directly into Facebook or WhatsApp

## Class Types

| Type | Description |
|------|-------------|
| **Pasos Básicos** | Beginner/fundamentals class |
| **Casino Royale** | Advanced partner work |
| **Choreo Team** | Performance team updates |
| **Special** | Cancellations, events, announcements |

## Repository Structure

```
scf-social-media/
├── README.md                    # This file
├── .claude/commands/
│   └── announce.md              # The /announce skill
├── docs/
│   ├── business-context.md      # SaborConFlow overview
│   ├── cuban-dance-terminology.md   # Dance glossary
│   ├── brand-voice-guide.md     # Tone and voice rules
│   ├── announcement-templates.md    # Structural templates
│   └── historical-examples.md   # Real announcement examples
└── output/                      # Saved announcements (optional)
```

## Brand Elements

**Greeting**: "Hey everyone!"

**Gratitude**: "Thank you for trusting me with your dance journey and showing up each week!"

**Signature**: "Sabor in every step, flow in every move 💫"

**Note**: Choreo Team messages have NO greeting, gratitude, or signature.

## Documentation

- `docs/business-context.md` - Business overview, location, classes
- `docs/cuban-dance-terminology.md` - Cuban dance terms glossary
- `docs/brand-voice-guide.md` - Complete voice and tone guidelines
- `docs/announcement-templates.md` - Templates for each class type
- `docs/historical-examples.md` - 18 real examples for reference

## Maintenance

To update the announcement style:
1. Edit `docs/brand-voice-guide.md` for tone changes
2. Edit `docs/announcement-templates.md` for structural changes
3. Add new examples to `docs/historical-examples.md`

The `/announce` skill reads these docs each time, so changes take effect immediately.
