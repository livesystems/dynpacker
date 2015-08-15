app-image-generator
=========

Generates AMIs with your application running on it using upstart and packer.

Install
-------

pip install app-image-generator

Usage
-----

Example command

```bash
app-image-generator <parent ami> <name of parent ami> <ami major version>-<ami minor version> <project name> \
<project version> <image revision, normally 1> <zip file of the app> <git commit id> <ci project name> <ci build name> \
-d <process type, e.g. web> -s <script to run, e.g. "python manage.py run_gunicorn -b 0.0.0.0:5000 -w 4"> \
-d <next process type> -s <script to run> -v
```

Speed up pip install
--------------------

Check out [wheelshop](https://github.com/KristianOellegaard/wheelshop#using-with-dynpacker)
