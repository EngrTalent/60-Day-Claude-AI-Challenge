🚀 Day 20 of My Claude AI Learning Journey by ABTalks

What I did:
I built a working camera-puzzle prototype into something closer to a real product, still one HTML file, still zero dependencies:
- Multi-profile login (up to 5 saved profiles + a guest mode) with its own stats per person
- A two-stage hint system (a quick 'peek' at the full photo, then a flash highlight of misplaced pieces)
- A full sound engine built from oscillators (Web Audio API, no audio files) plus haptic vibration on mobile
- A drag-and-drop photo upload fallback for when the camera is denied or unavailable
- A 'Countdown' game mode that races a clock instead of just timing you, with its own separate leaderboard
- A stats dashboard (win rate, streaks, best time and average moves per difficulty) and recent games log
- A 'Share Result' button and a downloadable result card image

What I learned:
- The Web Audio API can synthesise convincing UI sounds (pickup clicks, a win arpeggio) from raw oscillators. No audio files was needed.
- A cheap, dependency-free 'blur' for the shareable result card: draw the photo small, then stretch it back up. The upscaling itself does the blurring.
- Separating 'what belongs to the puzzle' from 'what belongs to the profile' is what actually made switching profiles mid-game possible without losing one's progress.

Result:
One self-contained HTML file that went from 'a puzzle game' to something with real product bones: profiles, sound, two hint types, two game modes, and a shareable result card, in my own orange-and-green colours.

<img width="1913" height="957" alt="Screenshot 2026-06-22 182149" src="https://github.com/user-attachments/assets/f52e19cd-d086-4213-8168-96bec2486b23" />
<img width="1918" height="941" alt="Screenshot 2026-06-22 182230" src="https://github.com/user-attachments/assets/6b313c4b-3e3a-41ad-a0b9-b192d720f14e" />
<img width="1903" height="946" alt="Screenshot 2026-06-22 182456" src="https://github.com/user-attachments/assets/a5bb612c-7c93-4a82-ab33-8a97339b02b0" />
