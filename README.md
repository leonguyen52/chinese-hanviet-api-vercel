## Overview

An API built using [json-server](https://github.com/typicode/json-server) that allows you to look up Chinese and Han Viet cognates, this original idea is started by [ryanphung](https://github.com/ryanphung) and I updated it to match my own requirements with new database.

It will be divided into 2 type "tughep" (2 chinese words) and "tudon" (single chinese word) while looking up dictionary.
* /tughep 23940x words
* /tudon 11411x words

## Demo

* https://xxx.vercel.app/tughep?word_like=可
* https://xxx.vercel.app/tughep?hanviet=trạng%20thái
* https://xxx.vercel.app/tudon?word_like=可
* https://xxx.vercel.app/tudon?hanviet=trạng%20thái

Also support rewrite, check in /api/server.js
* https://json-server-in.vercel.app/api/posts

![Powered by Vercel](https://images.ctfassets.net/e5382hct74si/78Olo8EZRdUlcDUFQvnzG7/fa4cdb6dc04c40fceac194134788a0e2/1618983297-powered-by-vercel.svg)

### How to use

1. Click "**Use this template**" or clone this repository.
2. Update or use the default [`db.json`](./db.json) in the repository.
3. Sign Up or login into [Vercel](https://vercel.com).
4. From the Vercel dashboard, click "**+ New Project**" then "**Import**" your repository.
5. In the "**Configure Project**" screen, leave everything default and click "**Deploy**".
6. Wait until deployment is done, and your own JSON server is ready to serve!


## Enable write operations

By default, only GET operation is allowed, thanks to the contribution by [@VicAv99](https://www.github.com/VicAv99) at [#6](https://github.com/kitloong/json-server-vercel/issues/6), we can now enable write operations as well.

You can find the example code in [`api/server.js`](./api/server.js).

## Reference

1. https://github.com/typicode/json-server
2. https://vercel.com
3. https://shadowsmith.com/how-to-deploy-an-express-api-to-vercel
4. https://github.com/ryanphung/chinese-hanviet-api
