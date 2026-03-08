# E-Mood-ji ✨

Turn your emojis into something magical — albums, bedtime stories, and constellations.

## Inspiration

E-Mood-Ji was inspired by the idea that emotions and moods can be translated into experiences. Instead of searching manually for something that fits how you feel, we wanted to build a playful tool that interprets emojis and recommends something meaningful in return.

By simply entering a few emojis, users can discover:
- Music albums that match their emotional landscape
- Constellations connected to the mood of the night sky
- Bedtime stories inspired by the symbols they chose

## What It Does
E-Mood-ji allows users to input a series of emojis and receive a recommendation based on the emotional meaning behind those symbols.

Depending on the selected category, the app can generate:

1. Album Recommendations
The system interprets emoji meanings (like nature, sadness, calmness, adventure) and recommends a music album whose themes match those emotions.

2. Constellation Matches
Users can explore constellations associated with mystery, strength, or cosmic wonder based on the emoji mood.

3. Bedtime Story Prompts
RX Remedy can generate a gentle bedtime story idea inspired by the emotional tone of the emojis.

## How We Built It
E-Mood-Ji was built as a lightweight web application using a simple but effective recommendation engine.

1. Frontend
- HTML
- CSS
- JavaScript

2. Data-driven recommendation system
We created a local dataset containing: albums, constellations, emoji meaning mappings. Each emoji is associated with a set of mood tags such as: calm, dreamy, nature, cosmic, etc.

When users enter emojis, the system:
- Converts each emoji into mood tags
- Combines all tags into a mood profile
- Scores items in the dataset based on how many tags match
- Returns the best recommendation

This allowed us to build a fast, no-API recommendation engine that works entirely from local JSON data.

## Challenges we ran into
1. We initially want to use Google Gemini API, however, we hit the rate limit. We had to pivot to using local dataset. It is more restricted in terms of albums, story, and constellation choices, but it gets the job done.
2. We also had to pivot from a different project as we ran into technical issues from the other project.

## Accomplishments that we're proud of
- Building a functional emoji interpretation system
- Creating a tag-based recommendation engine
- Supporting multiple content categories
- Designing a playful interface that encourages exploration

## What we Learned
- How to design data-driven recommendation systems
- How to structure JSON datasets for flexible matching
- How browsers handle local file security and fetch requests

## How to Run the Project Locally
1. Clone the project locally
- git clone https://github.com/lktran1105/e-mood-ji.git
- cd e-mood-ji
2. Start a local server: python3 -m http.server
3. Open the project in your browser: http://localhost:8000
