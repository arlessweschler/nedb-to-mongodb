# nedb-to-mongodb

If you've outgrown <a href="https://github.com/louischatriot/nedb" target="_blank">NeDB</a>, use this utility to transfer all your data in a nedb database in a MongoDB collection.

**IMPORTANT:** this uses by default the latest versions of nedb and the mongodb driver. If you're not using these the script may not work and you need to modify the `package.json`.

Please follow <a href="https://github.com/louischatriot/nedb#bug-reporting-guidelines">the NeDB bug reporting guidelines</a> if you submit an issue.

### Installation

```bash
git clone https://github.com/AndrewLaneX/nedb-to-mongodb.git
cd nedb-to-mongodb
npm install
```

### Usage

Usage is pretty straightforward. All the information you need is one `./transfer.js --help` away. Here is what this command tells you:

```
Usage: ./transfer.js [options]

Options:
  -V, --version                      output the version number
  -h, --mongodb-host [host]          Host where your MongoDB is (default: localhost) (default: "localhost")
  -u, --mongodb-username [username]  Username for your MongoDB user
  -p, --mongodb-password [password]  Password for your MongoDB user
  --mongodb-port [port]              Port on which your MongoDB server is running (default: 27017)
  -d, --mongodb-dbname [name]        Name of the Mongo database
  -c, --mongodb-collection [name]    Collection to put your data into
  -n, --nedb-datafile [path]         Path to the NeDB data file
  -k, --keep-ids [true/false]        Whether to keep ids used by NeDB or have MongoDB generate ObjectIds
                                     (probably a good idea to use ObjectIds from now on!)
  --help                             display help for command
```

### License

(The MIT License)

Copyright (c) 2013 Louis Chatriot &lt;louis.chatriot@gmail.com&gt;

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
'Software'), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
