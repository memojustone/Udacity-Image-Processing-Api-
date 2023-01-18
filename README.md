### Install dependencies
- Install: ```npm install```
- Build: ```npm run build```
- Lint: ```npm run lint```
- Prettify: ```npm run prettify```
- Run unit tests: ```npm run test```
- Start server: ```npm run start```


#### instructions
http://localhost:3000/

#### Examples
http://localhost:3000/api/images
Will display a hint and list available image names

http://localhost:3000/api/images?filename=fjord
Will display the original fjord image.

http://localhost:3000/api/images?filename=fjord&width=200&height=200
Will scale the fjord image to 200 by 200 pixels and store the resulting image.
On subsequent calls will serve the resized image instead of resizing the
original again.

http://localhost:3000/api/images?filename=fjord&width=-200&height=200
Invalid width parameter that will be hinted to.

http://localhost:3000/api/images?filename=fjord&width=200
Missing height parameter that will be hinted to.
