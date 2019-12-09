# WEBPACK-LEARNING
Simple intro project for WEBPACK LEARNING

# STEPS
1.install Node.js
2.cmd prompt >goto project folder
3. npm init
    //package.json file is generated
4.npm install --save-dev webpack webpack-cli
    //node_modules created, with all dependency pkgs inside.
   // and as devdependencies these are added in pkg.json
5. Goto Package.json--> scripts-> Add this script:

   "build":"webpack --mode development --entry ./js/app2.js --output ./dist/bundle.js"
   //dist== distribution folder, which will be created auto by 7th step
6.rewrite js files with export and import 
  with entry file as app2.js , so import others into this app2.js .
  export from app.js  //check code
7.npm run build
    //create a dist folder inside our project folder , and inside it bundle.js
    WEBPACK-LEARNING > dist > bundle.js
8.<script src="dist/bundle.js"</script> 
//rewrite script line for app.js and app2.js as above

------
Extras: for minifying

9. "build:prod": "webpack <------------> -p"
10.npm run build:prod
