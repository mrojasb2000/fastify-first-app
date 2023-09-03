# How run typescript server

if the first one didn't work, or you have for some reason to keep module: "ESNext"
1- Add "type": "module" to package.json

2- Install ts-node npm i -g ts-node

3- Go to tsconfig.json and add the following:

{
"compilerOptions": {
"module": "ESNext",
"moduleResolution": "Node",
/_ ... your props ... _/
},
"ts-node": {
"esm": true
}
}
4- Run ts-node fileName.ts
