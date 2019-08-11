BitTorrent Client
=================

Simple BitTorrent client built with Python's asyncio

Usage
-----

### Command Line Interface

1. Start a daemon:

        torrent_cli.py start &

2. *(optional)* Look at a list of files in a torrent you want to download:

        torrent_cli.py show ~/Torrents/debian-8.3.0-i386-netinst.iso.torrent

3. Specify a download directory and add the torrent to the daemon:

        torrent_cli.py add ~/Torrents/debian-8.3.0-i386-netinst.iso.torrent -d ~/Downloads

    If the torrent contains more than one file, you can select which files you want to download
    using `--include` and `--exclude` options. For more information run:

        torrent_cli.py add --help

4. Watch torrent status:

        watch torrent_cli.py status

    Add `-v` to increase output verbosity.

    You also can add more torrents, pause, resume, and remove them. For more information run:

        torrent_cli.py --help

5. To stop the daemon run:

        torrent_cli.py stop

    The daemon will restore its state after restart.

Available on PyPI: 
------------------

* [torrent-client](https://pypi.org/project/torrent-client/)
        pip install torrent-client


Acknowledgements: 
-----------------

* [Borzunov](https://github.com/borzunov/bit-torrent) - The Downloading portion of client! 

