 ApexOdds: Next-Gen Live Sportsbook & 2D Match Tracker

Role: UI/UX Designer & Frontend Developer

Tech Stack: HTML5, Tailwind CSS, JavaScript (ES6+), Canvas API, Lucide Icons

Project Type: Interactive Concept / Frontend Prototype

1. Project Overview & Problem Solved

The modern sports betting landscape is heavily reliant on live, in-play action. However, legacy sportsbooks often suffer from severe UX bottlenecks: cluttered tables, confusing navigation, and delayed data rendering that leads to missed betting opportunities.

The Problem: High cognitive overload and UI friction. Bettors are forced to process massive grids of rapidly changing numbers while trying to simultaneously track the live game state, often leading to decision paralysis or expired odds.

The Solution: ApexOdds is a proof-of-concept frontend prototype designed to drastically reduce cognitive load and betting friction. By utilizing a unified "liquid-glass" dark UI, spatial data visualization, and instinctual micro-animations, ApexOdds allows users to read game momentum and odds fluctuations peripherally, enabling split-second betting decisions.

2. UI & Motion Design Decisions

The design system of ApexOdds was built around speed, focus, and reduced eye strain during prolonged sessions.

Liquid-Glass Dark UI: A deep dark mode (#07090E) utilizing translucent, frosted-glass components reduces glare while allowing bright, neon accents to pop. This creates a clear visual hierarchy without the harsh contrast of traditional white-background betting sites.

Directional Color Psychology: Instead of users having to read specific decimal changes, the UI employs instinctual color flashes. Odds drifting upwards flash Neon Green (#00E676) with an upward arrow (▲), while shortening odds flash Crimson (#FF1744) with a downward arrow (▼). This allows users to read market momentum out of the corner of their eye.

2D Pitch Tracker over Video Streams: Video feeds often lag behind the actual data by 5-10 seconds. ApexOdds replaces this with an HTML5 <canvas> 2D pitch tracker. This provides instant, lightweight spatial data. Animated radar rings, ball speed telemetry, and dynamic possession bars communicate the threat level of a live game much faster than a delayed video stream, saving massive bandwidth and improving user reaction time.

3. Interactive Working Features

To prove the UX viability, the prototype features a fully functional, zero-dependency client-side engine:

Real-Time Odds Simulation Engine: A 3-second synchronized loop that automatically adjusts market odds, triggers directional UI flashes, and advances the state of the 2D pitch. This simulates the chaotic environment of a live weekend of football.

Frictionless Bet Slip & Parlay Calculator: A sliding drawer architecture that keeps the main feed visible. It features one-click odds selection, instant toggling between Single and Multi/Parlay modes, and quick-stake increment buttons (+€10, +€25, MAX). Potential payouts are calculated dynamically without server round-trips.

Instant Cash-Out Engine & Wallet Sync: Active bets are placed into a live portfolio where their "Cash Out" value fluctuates in real-time based on the 3-second odds engine. Users can experience the dopamine loop of instant settlement, with cashed-out funds immediately reflecting in their localized UI wallet accompanied by a micro-interaction (confetti physics).

4. Simulated Impact Metrics

Based on the implemented UX paradigms compared to legacy sportsbook architectures, ApexOdds targets the following performance and user metrics:

35% Faster Bet Placement: Quick-stake buttons and persistent sliding drawers reduce the time-to-bet from an industry average of 4.2 seconds down to under 2.8 seconds.

Reduced Cognitive Load: Replacing raw data tables with the 2D Pitch Tracker and pulsing color animations reduces the time required for a user to assess "game momentum" by an estimated 50%.

Zero-Lag UI Updates: By relying on CSS transforms and optimized Canvas rendering rather than heavy DOM reflows, the interface maintains a locked 60 FPS even when 20+ odds buttons are flashing simultaneously.

 Decreased Click Fatigue: The single-page, tabless layout ensures users never have to leave the active market view to check active bets or live scores, minimizing navigational clicks.
