Tekken 3 Access 1.0.1
=====================

Screen reader support for the Tekken 3 PC port (Tekken3.exe). Speech goes
through Prism to your screen reader (NVDA etc.), or the Windows voice if no
screen reader is running.

HOW TO START
  Run "Play Tekken 3 Access.exe" in the game folder (not Tekken3.exe).
  It starts the game and loads the mod. You hear "Tekken 3 Access loaded".
  Nothing in the game folder is replaced. If the port is updated and the mod
  can no longer find the game's code, it says so and stays off.

NEW IN 1.0.1
  - The distance hum has a volume control: Shift+F1 louder, Control+F1
    quieter (10 steps; step 0 turns the hum off). It is a little louder by
    default than in 1.0. The level is remembered.
  - The hum and the other fight sounds now go silent while the pause menu
    or its command list is open, and come back when you return to the fight.

NEW IN 1.0 (since the test builds)
  - All mod sounds play cleanly and on time. Before, Windows chopped them
    into pieces and played them at little over half speed, which crackled.
  - The opening movie, every character's ending and the Jin and Kazuya
    movie after the first demo fight are described as they play (see
    Movies below). Theater mode is read.
  - Memory card saving and loading are read.
  - The distance hum and the stick health readouts keep working while you
    play with a controller, even if another window comes to the front.
  - Tekken Ball: when the ball flies deeper than the opponent, a low swoop
    plays and each ping gets a soft echo while it stays behind them. F1 says
    "behind the opponent". Shift+F3 (experimental) swaps the pings for one
    continuous tone whose pitch rises and falls with the ball's height, and
    back.
  - Tekken Force: health items on the floor ring a soft bell, panned to their
    side, faster as you get closer, a step higher when the item is further
    back, lower when nearer the front. Picking one up plays three rising
    notes. F1 lists items too. Enemy beeps now speed up much more as an
    enemy closes in.

WHAT IS READ
  - Main menu: each mode as you move (Arcade, Team Battle, Time Attack,
    Survival, Tekken Ball, Tekken Force, Practice, Option, Theater), read
    from the game's own list, so unlocked modes are named correctly. VS mode
    only appears when a second controller is plugged in.
  - Character select: the name under your cursor. In Practice, picking the
    opponent reads "Opponent:" and then each name as you move.
  - Text menus (Practice mode menus, the pause menu, options): the menu
    title, the highlighted item, and its value; when you change a value
    only the new value is read.
  - Versus screen: "Yoshimitsu versus Law. Stage 1".
  - Announcements: Round 1, Ready, K O, You win / You lose, Time up,
    Continue countdown, Game over.
  - Command list (move list): Practice > Combo Training or VS CPU >
    Command List, and the Practice pause menu. Each move is read as you
    scroll: name, then the inputs, then "3 of 20". Up and down move one
    move, left and right jump five.
    Inputs use Tekken numbers: 1 left punch (Square), 2 right punch
    (Triangle), 3 left kick (Cross), 4 right kick (Circle). "1 plus 2" means
    press both together. Commas separate inputs. "hold forward" is the
    game's yellow arrow. "stance 1" is the game's circled 1: a move marked
    "stance 1" puts you in a stance, and moves "From stance 1" are done from it.
    The list is written for facing right: forward is right.
  - Health: "Health below half" and "Health low" warnings during fights.
  - Movies: the opening and every character's ending are described as
    they play, each line timed to the movie's own frames, in a recorded
    voice, and the game's sound dips under each line so it is easy to hear.
    The text is in T3Access\movies.txt and the recordings in T3Access\ad.
    To hear the lines with your screen reader instead, create an empty file
    T3Access\ad_reader.txt.
  - Theater mode: the movie under the cursor is read ("Jin Kazama. Dirty
    Blood"; "locked" for one you haven't earned). Start plays it.
  - Option mode: every menu and value ("Game option. Difficulty level,
    Medium"; "Round time, Infinite"); when you change a value, the new value.
    Key configuration, Memory card, and the Records pages (read when they
    open and when you turn a page with Left / Right; the win counts on pages
    2 and 3 are pictures and are not read yet).
    Memory card: Card save and Card load read their prompt ("Save: press
    Start. Cancel: press Square, Triangle, Cross or Circle") and the result
    ("Saved", "Loaded", "No memory card!", "Card is full!", "Cancelled").
    F11 now also reads that result text.
  - Team Battle: the team size ("Team size: 4", Left and Right change it),
    then the grid: each name, "Nina picked, 2" when you pick, and
    "Nina, picked" when you pass a fighter already on your team.
  - Time Attack clear: every stage time and your total ("Your time, 1
    minute 36.26 seconds. New record!").
  - Survival results: your number of wins.
  - New record name entry (after Time Attack or Survival): your place and
    time or wins, then "Letter 1, A". Left and Right choose the letter (read
    as you go: "B", "space", "dot"), Cross confirms it and moves to the next
    ("Letter 2, B"); the third Cross saves it ("Name saved: CB."). The time
    left is spoken at 10 and 5 seconds.

SOUNDS
  - One-on-one fights: a soft hum while a round is being fought (from
    "Ready" until K O, Time up and so on; silent in the pause menu, its
    command list and practice menus). Shift+F1 and Control+F1 make it
    louder and quieter.
    Higher = closer: about 190 Hz at the start of a round, rising to 330 Hz
    when you are touching, falling to 110 Hz when far apart.
    It leans to your forward side and changes with it: steady when
    forward is Right, gently pulsing when forward is Left. "Forward is left" /
    "Forward is right" is spoken when it changes during a round. This is the
    game's own setting, so it always matches which way Right and Left move you.
  - Sidesteps: a short sweep. Rising = sidestep up (into the screen, what
    pressing up does), falling = sidestep down. Your sidesteps are a clear,
    high sweep in the middle; your opponent's are a lower, buzzy sweep from
    their side.
  - Tekken Force: each enemy on screen beeps from its side, hard left or
    hard right. Faster = closer. Higher pitch = further up the screen (back),
    lower = nearer the front.
    The first enemy is a round tone, the second a buzzier one. Foot soldiers
    are not announced by speech; bosses are named.
    Boss fight at the end of a stage: the distance hum and the
    sidestep sweeps, as in one-on-one fights.

TEKKEN BALL
  Selecting: the character grid speaks each character as you move ("Locked"
  for one you have not unlocked yet), then the ball: Beginner beach ball
  (60 percent damage), Expert gum ball (80) or Grand Master iron ball (100).
  The court: the net is in the middle, you play on the left half and the
  opponent on the right. Players can't cross the net. The court is very
  narrow up and down the screen. A ball that lands close to the net
  bounces; one that lands further back on your half loses you the point
  and 30 health.
  Press F4 to hear every ball sound with an explanation (press again for
  the next one). There are three kinds of sound, each answering one question:
  1. Where is the ball? A soft two-note ping.
     - Left and right: where the ball is compared to you.
     - The first note never changes. The second note tells the height:
       the SAME note twice = the ball is at hitting height; a little higher =
       above your head; higher still = high; an octave = very high. As the
       ball drops toward you, you hear the two notes come together.
     - Faster pings = the ball is nearer. Slow, quiet, dull pings = the ball
       is going away on the opponent's side.
     - Rasping pings = a heavily charged ball ("Heavy ball" is also spoken).
  2. Where do I stand? While the ball is coming down on your half, a soft
     hum comes from the side of the spot you should stand on, rising as you
     get closer. On the spot it opens into a warm chord: stay there.
     A pulsing hum = the ball would land in your point zone (you must hit it).
     A short rising chirp = also step up (into the screen), falling = step down.
  3. When do I press? Once the ball's path comes into your reach: three
     beats in a steady rhythm. Press attack on the third, higher beat. If the
     third beat is LOW, the ball will be low (near your knees): use a kick.
     The pings stop during the beats so you can hear them.
     Too early or too late? Shift+F4 makes the beats earlier, Control+F4
     later (17 milliseconds per press; remembered).
  Other sounds: a bright tock when you hit the ball, a dull thud from their
  side when the opponent does, a low bump when it bounces near the net,
  "Point won" / "Point lost" with a short tune, "Hit by the ball" with the
  damage, a low bump behind you at the back line and a soft double tone in
  front at the net.
  F1 (or L3 and R3 together) says where you are and where the ball is, for
  example "Your half, middle. Ball high, in front, 12, landing on your side,
  point zone".
  Tested with a test player inside the mod that only followed these sounds
  (walk toward the hum, press on the third beat): it hit about two thirds of
  the balls coming to it and won points against the computer.
  The opponent distance hum and sidestep sweeps are off in Tekken Ball.

KEYS (keyboard)
  F1   distance to the opponent and which way is forward
       ("mid range, 20. Forward is right"; a round starts at 20),
       or in Tekken Force the enemies with distance and side,
       or in Tekken Ball where you are and where the ball is
  Shift+F1 / Control+F1  distance hum louder / quieter ("Distance hum 8 of
       10"; 0 turns it off; remembered). Outside a fight you hear the hum
       briefly at the new level.
  F2   health of you and your opponent
  F3   fight sounds on or off
  F4   Tekken Ball sound guide (each press plays the next sound and explains
       it); Shift+F4 / Control+F4 make the swing beats earlier / later
  F5   read the highlighted menu item again
  F11  read all text on the screen
  F12  repeat the last thing spoken
  The port itself uses Escape (its menu), F6, F7 (save states), F8, F9,
  Tab and F, so the mod stays off those.

CONTROLLER
  The port only uses a controller when settings.toml says so:
  p1_device = "auto" (the first connected controller). With that setting
  the keyboard no longer controls the game, but the mod's F keys still
  work. To go back to keyboard play, change it to p1_device = "keyboard".
  ("Use controller.bat" and "Use keyboard.bat" in the game folder do this.)
  Xbox, PlayStation 5 (DualSense), PlayStation 4 and most other controllers
  work, by cable or Bluetooth.

  Game buttons on an Xbox controller (Tekken numbers in brackets):
    X = Square, left punch (1)      Y = Triangle, right punch (2)
    A = Cross, left kick (3)        B = Circle, right kick (4)
    D-pad or left stick = move      Start = start / pause
    A or Start confirms in menus. Back = Select (used in Practice mode).
    LB, RB, LT, RT = L1, R1, L2, R2 (the port's input.ini can change these).
  On a PlayStation controller the buttons are the game's own: Square,
  Triangle, Cross, Circle, Options = start / pause, Create = Select.

  Mod buttons (Xbox and PlayStation controllers):
  L3 (click left stick)    your health ("You, 80 percent")
  R3 (click right stick)   your opponent's health ("Jin, 45 percent"; in
                           Tekken Force, each enemy on screen)
  L3 and R3 together       same as F1 (distance, enemies, or the ball)
  Outside fights: L3 reads the screen (F11), R3 the highlighted menu item
  (F5), both together read the screen.

SOUND DELAY
  The port keeps a long queue of game sound (180 ms by default), so hits and
  footsteps came noticeably after your button presses. The mod shortens it
  to 60 ms. If the game's sound ever crackles or breaks up, create a text
  file T3Access\audio_ms.txt containing a bigger number, for example 100
  (allowed 30 to 500), and restart.
  Graphics card: on computers with two graphics chips (most gaming laptops),
  the launcher asks Windows to run Tekken3.exe on the faster one, the first
  time you play. If you already picked a setting for Tekken3.exe in Windows
  Settings > Display > Graphics, your choice is kept.

NOT DONE YET / PLEASE REPORT
  - Character endings: the descriptions were checked from Theater mode, but
    not every character's ending has been played after finishing Arcade yet.
    If an ending is silent, wrong or out of step, please report it with
    T3Access\T3Access.log.
  - VS mode (needs a second controller) has not been checked.
  - Key configuration: the list that opens when you press a button to
    reassign it is read, but briefly; the port's own input.ini is simpler.
  - Tekken Force: the boss fight sounds and the health item pickup sound
    have not been tested in a full run yet.

FILES
  T3Access\T3Access.dll   the mod
  T3Access\prism.dll      speech
  T3Access\T3Access.log   what the mod did and said (send this with problem reports)
  T3Access\launch.log     what the launcher did
  T3Access\hum_volume.txt the distance hum volume you chose (made when you
                          first change it; delete it for the default)
