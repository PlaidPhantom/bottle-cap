# Cap

Lightweight Python3-compatible SQLite-based authentication framework for Bottle web applications

I built this because [Cork](http://cork.firelet.net/) did not (at the time) support Python 3. That seems to have been
remedied recently, but perhaps someone will still find this useful.  Feel free to make suggestions/pull requests/issues
and I'll look into them as I can!


## Dependencies

* [Bottle](http://bottlepy.org/)
* [Cryptography](https://cryptography.io/)


## Demo

`demo.py` is a small demonstration Bottle web app which uses a number of features of the Cap plugin.  Until I finish
the full documentation, refer to that for basic plugin usage.

To run the demo app:

1. Install dependencies (if not using pip, follow the appropriate package installation instructions for your environment):
    * `pip install bottlepy`
    * `pip install cryptography`
2. Run cap.py as a script to initialize a user database (run `python cap.py` to see options):
    * `python cap.py --db-path users.db --add-user test --add-user admin --create-role admin --add-role admin admin`
    * enter passwords for each user as prompted
3. Run the demo application
    * `python demo.py`
4. Access the application at `http://localhost:8080/`
