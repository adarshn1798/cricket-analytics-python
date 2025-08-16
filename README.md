**IPL Venue Analysis – Venue, Phase & Opposition Based Player Evaluation**
**Project Overview**
This project performs a venue analysis of IPL batters to evaluate their performance under specific match contexts.
By combining venue, phase of play, and opposition team, the analysis helps answer scouting questions like:

“How good is Player X at Chepauk in the middle overs against CSK?”
**Objectives**
1. Build a framework to analyze batting performance contextually.
2. Derive advanced batting metrics such as Strike Rate, Runs Per Innings, Balls Per Boundary, Dot %, etc.
3. Create a weighted composite score to rank batters fairly across multiple dimensions.
4. Generate shortlists of top players for targeted scenarios (e.g., auction scouting, matchups).
**Methodology**
**Data Sources**

deliveries.csv → Ball-by-ball IPL data
matches.csv → Match-level data (venue, teams, date, etc.)
**Feature Engineering**

**Metrics**: SR, RPI, Balls Per Dismissal, Balls Per Boundary, Dot%
**Context filters**: Venue, Phase (Powerplay, Middle, Death), Opposition Team
Scoring System

Apply weights to each metric (SR: 13%, RPI: 27%, BPD: 16%, Dot%: 45%)
Normalize values using squared distances (TOPSIS-inspired approach)
Compute a final composite score (0–1)
**Output**

Ranked list of top batters for the selected scenario
Insights into which players are most effective in given conditions
**Why This Project?**
In T20 cricket, performance varies heavily by venue conditions, match phases, and oppositions.
This framework helps scouts, analysts, and coaches make data-driven decisions in auctions, strategy, and player matchups.
