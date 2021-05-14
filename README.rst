mps-youtube-hd
==============


Fork Features
-------------
- View videos in resolutions higher than 360p, for instance 1080p. This is done
  by using mpv youtude-dl backend, rather than extracting a single stream.
- Works with mpv ytdl-format scripts, like `mpv-youtube-quality
  <https://github.com/jgreco/mpv-youtube-quality>`_.
- Requires mpv.
- Available in the `AUR
  <https://aur.archlinux.org/packages/mps-youtube-hd-git/>`_.

Features
--------
- Search and play audio/video from YouTube
- Search tracks of albums by album title
- Search and import YouTube playlists
- Create and save local playlists
- Download audio/video
- Convert to mp3 & other formats (requires ffmpeg or avconv)
- View video comments
- Works with Python 3.x
- Works with Windows, Linux and Mac OS X

This project is based on `mps
<https://web.archive.org/web/20180429034221/https://github.com/np1/mps>`_, a
terminal based program to search, stream and download music.  This
implementation uses YouTube as a source of content and can play and download
video as well as audio.  The `pafy <https://github.com/mps-youtube/pafy>`_
library handles interfacing with YouTube.

`FAQ / Troubleshooting common issues
<https://github.com/mps-youtube/mps-youtube/wiki/Troubleshooting>`_

Screenshots
-----------


Search
~~~~~~
.. image:: http://mps-youtube.github.io/mps-youtube/std-search.png

A standard search is performed by entering ``/`` followed by search terms.

You can play all of the search results by giving ``1-`` as input

Repeating song/songs can be done with ``song_number[loop]``, for example: ``1[3]`` or ``4-6[2]``

Local Playlists
~~~~~~~~~~~~~~~
.. image:: http://mps-youtube.github.io/mps-youtube/local-playlist.png

Search result items can easily be stored in local playlists.

YouTube Playlists
~~~~~~~~~~~~~~~~~
.. image:: http://mps-youtube.github.io/mps-youtube/playlist-search.png

YouTube playlists can be searched and played or saved as local playlists.

A playlist search is performed by ``//`` followed by search term.

Download
~~~~~~~~
.. image:: http://mps-youtube.github.io/mps-youtube/download.png

Content can be downloaded in various formats and resolutions.

Comments
~~~~~~~~
.. image:: http://mps-youtube.github.io/mps-youtube/comments.png

A basic comments browser is available to view YouTube user comments.

Music Album Matching
~~~~~~~~~~~~~~~~~~~~

.. image:: http://mps-youtube.github.io/mps-youtube/album-1.png

.. image:: http://mps-youtube.github.io/mps-youtube/album-2.png

An album title can be specified and mps-youtube will attempt to find matches
for each track of the album, based on title and duration.  Type ``help search``
for more info.

Customisation
~~~~~~~~~~~~~

.. image:: http://mps-youtube.github.io/mps-youtube/customisation2.png

Search results can be customised to display additional fields and ordered by
various criteria.

This configuration was set up using the following commands::

    set order views
    set columns user:14 date comments rating likes dislikes category:9 views

Type ``help config`` for help on configuration options



Installation
------------

Arch Linux
~~~~~~
You can install mps-youtube-hd from the AUR (``mps-youtube-hd-git``).


Usage
-----

mps-youtube is run on the command line using the command::

    mpsyt

Enter ``h`` from within the program for help.
