to install and run this on your local device you need to run the following comands 

```bash
npm install --legacy-peer-deps @react-three/fiber @react-three/drei maath react-vertical-timeline-component @emailjs/browser framer-motion react-router-dom
```



also when doing this you can get an issue with the version specified for the react-tilt package in your package.json

to resolve this you need to do the following steps 
##  <a name="table">Resolving the React-tilt-Version error</a>
1. go to your package.json

   
2.you will se a code like this 
```bash
    {
        "dependencies": {
         "react-tilt": "^<new_version>",
           ...
       }
     }
```
3. change it to 
```bash
      {
             "dependencies": {
             "react-tilt": "^0.1.4",
              ...
          }
       }
```
then after this you need to run 

```bash
npm install --legacy-peer-deps @react-three/fiber @react-three/drei maath react-vertical-timeline-component @emailjs/browser framer-motion react-router-dom
```

if this doesn't work you have to run it with force 
```bash
npm install --force @react-three/fiber @react-three/drei maath react-tilt react-vertical-timeline-component @emailjs/browser framer-motion react-router-dom
```
  and then isntall 
  ```bash
npm install vite
```
and then
```bash
npm run dev
```
##
if the above way doesn't work then you have to remove the react-tilt  

so the installation codes becomes 
```bash
npm install --legacy-peer-deps @react-three/fiber @react-three/drei maath react-vertical-timeline-component @emailjs/browser framer-motion react-router-dom
```

then
```bash
npm install vite
npm run dev
```

if you have anyother way to run feel free to add it in this readme and help me and others



