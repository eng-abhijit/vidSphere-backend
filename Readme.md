
fir install -  "devDependencies": {
    "nodemon": "^3.1.10",
    "prettier": "^3.5.3"
  },

  then install  "dependencies": {
    "dotenv": "^16.5.0",
    "express": "^5.1.0",
    "mongoose": "^8.16.0"
  }

  package.json file- 

  "type": "module",
    "scripts": {
    "dev": "nodemon src/index.js",
    "start":"node src/index.js"
  },


--prettierignore--
/.vscode
/node_modules
./dist

*.env
.env
.env.*

--.prettierrc------------------
{
    "singleQuote": false,
    "bracketSpacing": true,
    "tabWidth": 2,
    "trailingComma": "es5",
    "semi": true
}

db connection code : index.js file ---------------
/*
import dotenv from "dotenv";
dotenv.config();
import mongoose from "mongoose";
import {DB_NAME} from "./constrants.js";
import express from "express";
const app=express();

;(async()=>{
   try {
   await mongoose.connect(`${process.env.MONGODB_URL}/${DB_NAME}`);
    app.on("error",(err)=>{
      console.log(err);
    });
    app.listen(process.env.PORT,()=>{
        console.log(`server runnting on ${process.env.PORT}`);
    })
    
   } catch (error) {
    console.log("ERROR: " + error);
   }
})();

*/
