# Pencil desktop launcher

I needed to run [Pencil](https://github.com/evolus/pencil) through a desktop launcher, because I don't wanted move on to the Pencil's directory and run ```npm start``` everytime I wanted to use it.

Then I created a simple script to solve that in a file called pencil, and I put it into ```/usr/local/bin```. 

It basically uses [```npm start --prefix```](https://docs.npmjs.com/misc/config#prefix) to pointing to a place from where it must be run, and nohup to run it in background leaving the terminal free.

You can redirect output message to ```/dev/null 2>&1 &``` if you want as well.

Don't forget to replace ```/path-to/pencil``` of pencil file by your system path to Pencil, and give it executable permission.

## Acknowledgement

* [Pencil Project](https://github.com/evolus/pencil)