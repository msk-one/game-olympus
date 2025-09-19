# Game Olympus

> AI-powered relationship-driven visual novel where players become deities navigating modern Olympian society.

## Project Overview

**Game Olympus** combines sophisticated relationship mechanics with dynamic AI-generated content to create personalized mythological narratives. Players make choices that affect divine relationships, unlock story branches, and shape their path through a world where ancient gods operate in contemporary settings.

For complete game mechanics and flow details, see [Game Details](game_olympus.md).
Full GDD (Game Design Document) at [Game Design Document](game_olympus_gdd.md).

## Technical Stack

### Unity 6.2 Foundation
Built on Unity 6.2 with Universal Render Pipeline for optimal mobile performance and sophisticated 2D visuals. Modular architecture enables rapid hackathon development and easy debugging.

### Partner Tool Integration

#### [Redis](https://redis.io/)
Stores all player choices, relationship scores, and story flags. Enables real-time relationship tracking and cross-session memory that makes every choice meaningful.

#### [Apify](https://apify.com)
Scrapes authentic Greek mythology sources to generate procedural quests and storylines. Transforms static myths into contextual game content based on player relationships.

#### [Minimax](https://www.minimax.io/)
Real-time voice synthesis that changes based on relationship dynamics. Characters sound warmer or colder depending on player choice history.

#### [BrightData](https://brightdata.com/)
Cross-references mythology content against academic sources to ensure respectful and authentic representation of Greek culture.

#### [Winter Comics](https://www.wintercomics.com/)
AI-generated character expressions, outfits, and environments that maintain visual consistency while responding to story developments.

## Project Structure

```
GameOlympus/
├── Assets/
│   ├── Art/                    # Winter Comics assets
│   ├── Audio/                  # Minimax voice content  
│   ├── Scripts/
│   │   ├── Core/              # Game management systems
│   │   ├── Characters/        # Relationship mechanics
│   │   ├── Dialogue/          # Conversation system
│   │   └── External/          # API integrations
│   └── Data/                  # Game content and configs
├── gameolympus.md             # Game details and mechanics
└── README.md                  # README for project
```

## Quick Setup

### Prerequisites
- Unity 6.2+ with Universal Render Pipeline packages
- API access for: Redis, Apify, Minimax, BrightData, Winter Comics

### Installation
```bash
git clone [repository-url]
cd GameOlympus
# Open in Unity 6.2
```

### Required Unity Packages
- Visual Scripting
- Timeline  
- TextMeshPro
- 2D Animation
- Newtonsoft Json

## Development Phases

Trailer, core systems + basic dialogue flow >>> Redis integration + relationship tracking >>> Apify content generation + BrightData validation >>> Minimax voices + Winter Comics assets + polish

## Build Targets

- **Development**: PC/Mac standalone for testing
- **Production**: Mobile (iOS/Android) via Progressive Web App
- **Demo**: WebGL build for hackathon presentation (hopefully!)

## Key Features

- **Persistent Relationships**: Every choice affects future interactions
- **Dynamic Content**: AI-generated quests from authentic mythology  
- **Adaptive Audio**: Character voices reflect relationship status
- **Cultural Authenticity**: Validated mythological references
- **Visual Consistency**: AI-generated assets matching established style

## Demo Flow

1. **Character Creation** - Design your deity
2. **First Encounter** - Meet Hades at Underworld  
3. **Choice Impact** - Make decision affecting relationship
4. **Voice Response** - Hear Minimax-generated reaction
5. **Consequence Display** - See Redis-stored relationship change

---

Read [Game Details](game_olympus.md) then follow the setup guide above.