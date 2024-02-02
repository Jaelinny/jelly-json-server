# jelly-json-server
![](https://raw.githubusercontent.com/onevcat/lgtm-images/master/images/Jjf6ckr.png)

### RUN
```
$ npx json-server db.json

JSON Server started on PORT :3000
Press CTRL-C to stop
Watching db.json...

(˶ᵔ ᵕ ᵔ˶)

Index:
http://localhost:3000/

Static files:
Serving ./public directory if it exists

Endpoints:
http://localhost:3000/posts
http://localhost:3000/comments
http://localhost:3000/profile
```
### Launch
- ⚠️ Do you want to tweak these settings before proceeding? Yes
```
flyctl launch
Scanning source code
Detected a Dockerfile app
Creating app in /home/jelly/code/jelly-json-server
We're about to launch your app on Fly.io. Here's what you're getting:

Organization: _꾸꾸                (fly launch defaults to the personal org)
Name:         jelly-json-server      (derived from your directory name)
Region:       Tokyo, Japan           (this is the fastest region for you)
App Machines: shared-cpu-1x, 1GB RAM (most apps need about 1GB of RAM)
Postgres:     <none>                 (not requested)
Redis:        <none>                 (not requested)

? Do you want to tweak these settings before proceeding? Yes
failed opening browser. Copy the url (https://fly.io/cli/launch/4779e8ec31016f7625be514308eff729) into a browser and continue
Waiting for launch data... Done
Created app 'jelly-json-server' in organization 'personal'
Admin URL: https://fly.io/apps/jelly-json-server
Hostname: jelly-json-server.fly.dev
? Create .dockerignore from 1 .gitignore files? Yes
Created /home/jelly/code/jelly-json-server/.dockerignore from 1 .gitignore files.
Wrote config file fly.toml
Validating /home/jelly/code/jelly-json-server/fly.toml
Platform: machines
✓ Configuration is valid
==> Building image
Remote builder fly-builder-snowy-silence-8109 ready
Remote builder fly-builder-snowy-silence-8109 ready
==> Building image with Docker
--> docker host: 20.10.12 linux x86_64
[+] Building 254.2s (9/10)
 => [internal] load build definition from Dockerfile                                   0.5s
 => => transferring dockerfile: 201B                                                   0.5s
 => [internal] load .dockerignore                                                      0.6s
 => => transferring context: 103B                                                      0.5s
 => [internal] load metadata for docker.io/library/node:20.11                          1.1s
 => [internal] load build context                                                      0.9s
 => => transferring context: 373B                                                      0.6s
 => [1/5] FROM docker.io/library/node:20.11@sha256:fd0115473b293460df5b217ea73ff216  252.5s
 => => resolve docker.io/library/node:20.11@sha256:fd0115473b293460df5b217ea73ff21692  0.1s
 => => sha256:5b9fe7fef9befda786bc8e1dd1ae42ffd8b9c37a4cce3c433e 211.11MB / 211.11MB  22.4s
 => => sha256:278d467c182fb935287ed6f4be3d44f8ac2714264bcb58b883d0cd2 3.37kB / 3.37kB  0.4s
 => => sha256:723a77f71cf06aeaa21ea74bfc1299e8362d26db488a7fba4e8b744 7.34kB / 7.34kB  0.0s
 => => sha256:6a299ae9cfd996c1149a699d36cdaa76fa332c8e9d66d6678fa9a 49.58MB / 49.58MB  5.8s
 => => sha256:fd0115473b293460df5b217ea73ff216928f2b0bb7650c5e7aa56aa 1.21kB / 1.21kB  0.0s
 => => sha256:c3e72880014551ecfe631aae3aef14ed33b7e58b4b682f5a3988381 2.00kB / 2.00kB  0.0s
 => => sha256:e08e8703b2fb5e50153f792f3192087d26970d262806b397049d 24.05MB / 24.05MB  15.3s
 => => sha256:9b5f63cb30c69fe1a827c8fea9d33bd7026dffa193ed449ff44e 47.99MB / 47.99MB  17.4s
 => => sha256:230542c909b8c810d61434d1f259307fac388dda9d2daca1aaf069c 2.21MB / 2.21MB  2.3s
 => => sha256:dc95f2a6ccee7fb934bd659ef134da3e3c71c2a4a8059fe3c79a7d230e6 450B / 450B  0.6s
 => => sha256:68e92d11b04ec0fe48e60d59964704aca234084f87af5d1a068c 64.14MB / 64.14MB  12.6s
 => => extracting sha256:6a299ae9cfd996c1149a699d36cdaa76fa332c8e9d66d6678fa9a231d9e  26.2s
 => => extracting sha256:e08e8703b2fb5e50153f792f3192087d26970d262806b397049d61b9a14b  5.7s
 => => extracting sha256:68e92d11b04ec0fe48e60d59964704aca234084f87af5d1a068c49456b3  20.8s
 => => extracting sha256:5b9fe7fef9befda786bc8e1dd1ae42ffd8b9c37a4cce3c433e65ebb890c  63.4s
 => => extracting sha256:278d467c182fb935287ed6f4be3d44f8ac2714264bcb58b883d0cd25754f  0.0s
 => => extracting sha256:9b5f63cb30c69fe1a827c8fea9d33bd7026dffa193ed449ff44e1c98189  16.2s
 => => extracting sha256:230542c909b8c810d61434d1f259307fac388dda9d2daca1aaf069c0b68a  0.7s
 => => extracting sha256:dc95f2a6ccee7fb934bd659ef134da3e3c71c2a4a8059fe3c79a7d230e65  0.0s
 => [2/5] WORKDIR /app                                                                 1.1s
 => [3/5] RUN npm install -g npm                                                      57.2s
 => [4/5] RUN npm install -g json-server                                              26.1s
 => [5/5] COPY ./db.json /app                                                          0.2s
 => exporting to image                                                                 2.5s
 => => exporting layers                                                                2.5s
 => => writing image sha256:4d7f2f1214ade49109977289143c769212a440f1a991045b6092024dc  0.0s
 => => naming to registry.fly.io/jelly-json-server:deployment-01HNMBFP7MY6E190VEWE9ZX  0.0s
--> Building image done
==> Pushing image to fly
```

### DEPLOY
```
$ fly deploy
```
### https://jelly-json-server.fly.dev/

### FROM
- https://www.npmjs.com/package/json-server
