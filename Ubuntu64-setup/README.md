Acronym Explanation:
--------------------

* M - Mongo.db is a no-sql database (really scalable)
* E - Express.js a framework for node.js (node.js is not a framework)
* A - Angular.js a quick way of creating webapps
* N - Node.js server-side javascript

The hope of this (and perhaps some Jade Templating) is to minimize the time and lines-of-code necessary for a site set-up and to maximize the maintability of a site.

**a side-goal is to get Node.js, which is actively developed and adds great future potential to a site


## Installing the Mean stack:

`cd` into the root directory, and let's begin start by installing Node.


### Installing Node 

This gets you the latest version of Node.js
```bash
sudo apt-get update
sudo apt-get install -y python-software-properties python g++ make
sudo add-apt-repository -y ppa:chris-lea/node.js
sudo apt-get update
sudo apt-get install nodejs
```

### Installing Express.js

Create a directory `node` with the following commands:

```bash
mkdir node
```

and `cd` into it with the usual:

```bash
cd node
```

Now we will get you express.js
```bash
npm install -g express
```

## Getting Mongo

Next go ahead and start a new session with express:

```bash
express --sessions HelloNodeExpress
```

go ahead and `cd` into the newly created HelloNodeExpress directory:

```bash
cd HelloNodeExpress
```


## Installing `Mongo` (and the helper `Monk`)

Next, we'll modify your `packages.json` file in the `HelloNodeExpress` directory, then use `npm` to install `Mongodb` and `Monk`

### Modding the `packages.json`

First, open with vim or your favorite text editor the `packages.json` file:

Then, change `packages.json` by adding two lines to the `dependencies` attribute (the lines with "monk" and "mongodb")

Your final product should look like this:

```json
{
    "name": "application-name",
    "version": "0.0.1",
    "private": true,
    "scripts": {
        "start": "node app.js"
    },
    "dependencies": {
        "express": "3.4.4",
        "jade": "*",
        "mongodb" : "*",
        "monk" : "*"
        
    }
} 
```

### You are finally ready to install Mongo! (and Monk!) 

Just type the following into the command line, and watch as npm magically finds and installs `monk` and `mongodb` :smiley:

```bash
npm install 
```

...type the above in and the installation should be well underway.

## Testing your app

To test your app run it with the following:

```bash
node app.js
```

(**Note you'll run your apps with `node` command) 

### Success!
If your setup was a success you should be able to find the following on your website on the specified port:

---

![Express Setup Success](Express_Success.png )

---

### Now Let's Customize It : )

Once you have something running it's usually easy to start modding it.

Go ahead and open up the `app.js` file with your text-editor, and change the heading:


```javascript



```




## References:

These notes are compiled mainly from the following sources:

* http://cwbuecheler.com/web/tutorials/2013/node-express-mongo/?src=hn
* 
