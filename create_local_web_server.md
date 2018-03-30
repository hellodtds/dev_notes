Ever received the following error message because we weren't directly hosting the images we wanted to display.

```
Uncaught SecurityError: Failed to execute 'toDataURL' on
'HTMLCanvasElement': Tainted canvases may not be exported.
There are couple of ways to get around this error and one (optionally) is to start a local web server. Below, I've outlined some different options for simple HTTP web server with instructions for setting them up.
```

## Python SimpleHTTPServer
Windows, Mac, Linux
[Download here](https://www.python.org/downloads/) (you may already have it installed!)
All you need is Python and a command line. Python comes with Mac and Linux but Windows users will need to download it. There are two main versions of Python, Python 2 and Python 3. Both are perfectly fine for setting up a simple server.

### Instructions
1. Open the terminal (Mac and Linux) or command prompt (Windows).
2. `cd` to a directory where you've saved an HTML file. For example, `cd ~/Documents/mysite/`. (Mac and Linux: here's more on cd if you aren't familiar with the terminal. Windows: here's more info on cd for you).
3. Run `python --version`. If Python is installed, you'll see "Python X.Y.Z". The "X" will be 2 or 3, indicating Python 2 or 3. If nothing shows up or the command produces an error, I recommend that you [download Python](https://www.python.org/downloads/).
4. If you have Python 2, run `python -m SimpleHTTPServer 8000`. If you have Python 3, run `python -m http.server 8000`.
5. Navigate your browser to `http://localhost:8000/`. If there is a file called `index.html` in the directory where you ran the command from step 4, then it should automatically show up! If not, you should see the files in that directory listed. Click on an HTML file and watch it load! Congrats! You've got a server running.
(What was that `8000`? It's a network port, which computers use to organize their network traffic.)

## MAMP
Windows and Mac
[Download here](https://www.mamp.info/) (you only need the free version!)
This is a simple GUI for serving a directory.

### Installation
Check out the [MAMP website installation instructions](https://documentation.mamp.info/documentation/mamp/).

## Node
Windows, Mac, Linux
Requires Node and npm (comes with node)
Similar to the Python technique above, this is a simple command line tool. This technique uses Node, which is a popular JavaScript runtime (i.e, a piece of software that runs arbitrary JavaScript outside of the browser). Node is incredibly popular for a number of uses, including servers. While Node rarely shows up in front-end work, every web developer will likely encounter its package installer, npm. npm (Node Package Manager) is a command line tool that makes it easy to install and manage other command line tools, libraries and frameworks.

This strategy may take a little more time to install than Python, but it's worth trying so that you get a head-start with npm. That being said, if you try this and run into problems, it's not a big deal - just use a different strategy.

### Installation
Run `node --version` from the terminal or command line. If nothing shows up or you get an error, install Node.
Run `npm install -g http-server`.
Serve files with h`ttp-server ~/Documents/mysite -p 8000` (replace `~/Documents/mysite` with the path to your project's directory!).
Navigate your browser to `http://localhost:8000` to test!