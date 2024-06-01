# PyMusicPlayer
A music player application written in Python, leveraging object-oriented programming (OOP) concepts for a structured and modular design. The application features a user-friendly interface built using Tkinter/PyGame, allowing users to play, pause, resume, and stop music tracks with ease.

**Importing Libraries:**

The code begins by importing necessary libraries: Tkinter for GUI components, ttk for themed widgets, filedialog for file browsing dialog, pygame for playing audio files, and os for interacting with the operating system.

***Class Definition**:
The code defines a class named MusicPlayer. This class encapsulates all the functionalities of the music player.

**Constructor Method (__init__):**

The __init__ method initializes the MusicPlayer object. It sets up the Tkinter root window, initializes Pygame and Pygame Mixer, and declares variables (track and status) to keep track of the current playing song and status, respectively.
It also creates frames for displaying song track and control buttons, as well as a playlist frame for displaying the list of songs.

**Methods:**
browse_music_directory: This method opens a file dialog to browse and select a directory containing music files. It then loads the music files from that directory into the playlist.
load_music_files: This method loads the music files from the selected directory into the playlist. It filters only .mp3 files and inserts them into the playlist.
playsong: This method retrieves the selected song from the playlist, sets the track and status variables, loads the selected song using Pygame Mixer, and starts playing it.
stopsong: This method stops the currently playing song.
pausesong: This method pauses the currently playing song.
unpausesong: This method unpauses the paused song.

**Creating TK Container and Running the Application:**

Outside the class definition, an instance of the Tkinter Tk class is created, which represents the main window of the application.
An instance of the MusicPlayer class is created, passing the root window (Tk instance) to it.
Finally, the main event loop (mainloop()) is started to run the Tkinter application.

**Connection to OOP Concepts:**

Encapsulation: The MusicPlayer class encapsulates all the functionalities related to the music player within a single class.
Abstraction: The class abstracts away the implementation details of playing music, interacting with the GUI, and managing playlists.
Modularity: The code is divided into smaller, manageable methods, each responsible for a specific functionality, promoting modularity.
Inheritance: Although not explicitly shown in this code, you could extend this class to add more features or customize its behavior further.
Polymorphism: Different methods (playsong, stopsong, pausesong, unpausesong) exhibit polymorphic behavior depending on the current state of the music player
