# Summary
## Piece 1: Audiovisualizer
The first piece I created was an audiovisualizer, which displays a frequency amplitude wave as the song plays. I used Java code (MidiToSynthSequence.java) to covert a MIDI file to a synthSequence file that only uses one instrument (SineEnv). I also removed percussion in post (just delete the percussion section in the data.txt output from the Java file). There are two demos in the ./tutorials/synthesis/bin folder, Galaxy.exe and Lake.exe, which showcase this program.
### Galaxy.exe
Song: Arrangement of Gusty Garden Galaxy from Super Mario Galaxy

Original Composer: Koji Kondo

MIDI File: https://www.vgmusic.com/file/98ed5cf946dba46cdcc7b589e87596a8.html
### Lake.exe
Song: Arrangement of Lake from Pokemon Diamond & Pearl

Original Composer: Go Ichinose

MIDI File: https://www.purezc.net/forums/index.php?showtopic=74076
## Piece 2: Piano Roll Interactable
Next, I wanted to create a MIDI piano roll using the AlloLib code. This piece is simply an interactive piano roll, which draws notes at locations based on their frequency and their lengths is is however long the user holds down the key. This piece demonstrates the use of timers to extend the lifespan of a note beyond when the sound of the note end.
### Piano.exe
No composition, just use the keyboard to play some notes (same control scheme as 01_SineEnv_Piano.cpp).
## Piece 3: Piano Roll MIDI
This piece is a non-interactive piano roll that plays a synthSequence file. I used a variation of the original Java code (MidiToSynthSequence2.java) to achieve the white notes appearing before the audio is played by adding "ghost" notes in the synthSequence file that play 4 seconds earlier than the actual note and have amplitude 0. My Piano_Roll_MIDI.cpp detects these as preluding notes and displays them accordingly. The actual notes have color, and are positioned and scaled to have the appearance of "filling" in the white note as the note plays.

The main limitation with this (and the previous piece) is that rendering all these notes, even if they do not have a sound, takes up a ton of CPU, and only really basic songs can be played without lag.
### Fairy.exe
Song: Arrangement of Great Fairy's Fountain from The Legend of Zelda: Ocarina of Time

Original Composer: Koji Kondo

MIDI Files: https://www.vgmusic.com/file/f1873dccfa37c5232aff5bcf7818c63c.html
## Piece 4: Rhythm Game
My final piece is more of a demonstration of interactivity and graphics over original composition. I created a simple rhythm game that can be played using the arrow keys. First, I studied Aviv's code to learn how to play .wav samples, which allowed me to play background music and sound effects for hits. I then created the main gameplay loop in the MyApp class, which draws all the notes, handles user input, keeps track of combos, and also draws the fun graphics. I created a beatmap by making a percussion MIDI in Musescore 3, then converting that MIDI to a .txt file using Java code (MidiToBeatmap.java), and then my code reads it and puts everything into a queue. The first demo is an alpha version of the rhythm game, which generates a random beatmap, while the second is more complete in terms of graphics and gameplay (support for held notes).

The main limitation with this piece is that the code is atrocious. Literally god-awful.
### AI Bomb.exe
Song: Artifical Intelligence Bomb

Original Composer: なると

Link: https://www.youtube.com/watch?v=4gtGeZ2wOmo

### Death by Glamour.exe
Song: Death by Glamour from Undertale

Original Composer: Toby Fox

Link: https://www.youtube.com/watch?v=2TgO-tN5wAM
