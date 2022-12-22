![This is an image](https://i.postimg.cc/pVDjhqRC/images-1.jpg)
‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎     ‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎     ‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎     ‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎     ‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎  ‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎     ‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎     ‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎     ‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎ ‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎     ‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎     ‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎     ‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎     ‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎     ‎‎‎   ‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎‎  ‎‎‎[api.leiamnash.com](https://web.leiamnash.repl.co/)

a free `api` for everyone that can be used in your program, this `api` provides random images, random quotes and many more
<br> <br>

#### requesting chatfuel
<br>

to request an chatfuel using my `api` you need to use a package, but before that, here are some examples of how to request on my `api`
<br>

- the first thing you need to do is code a join `text or query` for your program
<br>

- [ ] take note that this code is a simple example only, it depends on how your program works

> query example 
```ruby
https://api.leiamnash.repl.co/sim?chat=${req.query}
```

> after prefix example
```js
var prefix = event.body.slice(global.config.prefix.length).trim().split(/ +/);

var text = prefix.slice(1).join(" ");

(`https://api.leiamnash.repl.co/sim?chat=${text}`)
```

> if you're using the `mirai project`, don't forget to add args on top of modules. here's an example
```js
module.exports.run = async ({ args, event, api }) => {

var text = args.join(" ");

(`https://api.leiamnash.repl.co/sim?chat=${text}`)
} 
```

[ 𝗻𝗼𝘁𝗲 ] » this is not the full source code, this is just an example. if you copy this, it will remain an error because this is just a shortcut code and there are a lot of things missing here

- second step is you need to check is the output of my `api` but most of the output i used is an `answer`
> to check the output of my api, just click on the link or paste it into your browser
```ruby
https://api.leiamnash.repl.co/sim?chat=hello
```

here's an example of the output
![This is an image](https://i.postimg.cc/rpKZCzJ8/Screenshot-2022-1222-145540.png)

- request
```js
var img = res.data.answer;
```

to use my api link as a response, you need to use the `axios` package for more information please read the documentation of [axios read file](https://www.npmjs.com/package/axios)
<br>

[ 𝗻𝗼𝘁𝗲 ] » i am not providing a `full source code` here. i only made this as a guide for those who are newbies and don't know how to use my `api`. if you don't know how to make response, it's better to read the [axios documents](https://www.npmjs.com/package/axios)

<br>

#### requesting images 
<br> 

to request an image using my `api` you need to use a package, but before that, here are some examples of how to request on my `api`
<br>

- first thing you need to check is the output of my `api` but most of the output i used is an `image`
> to check the output of my api, just click on the link or paste it into your browser
```ruby
https://api.leiamnash.repl.co/rem
```

here's an example of the output
![This is an image](https://i.postimg.cc/VLH036wr/Screenshot-2022-1222-143600.png)

- request
```js
var img = res.data.image;
```

to use my api link as a response, you need to use the `axios` package for more information please read the documentation of [axios read file](https://www.npmjs.com/package/axios)
<br>

[ 𝗻𝗼𝘁𝗲 ] » i am not providing a `full source code` here. i only made this as a guide for those who are newbies and don't know how to use my `api`. if you don't know how to make response, it's better to read the [axios documents](https://www.npmjs.com/package/axios)

<br>

developer [Leiam Nash](https://facebook.com/LeiamNashRebirth)
