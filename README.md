JS Tooling
===================================
[![GitHub Classroom Workflow](https://github.com/IT3049C-Lively-FA23/Tooling-Lab-Template/actions/workflows/classroom.yml/badge.svg)](https://github.com/IT3049C-Lively-FA23/Tooling-Lab-Template/actions/workflows/classroom.yml)

Instructions to this assignment can be found [here](https://reedws.github.io/IT3049C/coursework/labs/tooling/).

## Checklist:
- [x] update the assignment checks above to the correct link. - Done Automatically
- [ ] make sure the assignment checks pass
- [x] fill out the self evaluation and Reflection
- [ ] submit the repository link on Canvas

## Self-Evaluation: 
how many points out of 10 do you deserve on this assignment: 
5
## Self-Reflection:
I tried to complete the labs but the instructions did not corelate with what I was seeing on my end. I tried to get it working with troubleshooting 

I am getting a couple issues with the lab for tooling lab this week and I wanted to share my problem with you to see if you could give me a suggestion on how to fix it.
First of all, the npm init @eslint/config command wouldn't allow me to select a file format for the config file. After running the command it would have me install dependencies and from there the output would be a eslint.congig.mjs file. After running the command again the same thing happened where I have to install dependencies and I wouldn't be given the option to save the config as a json file.

C:\Users\antd2\Desktop\Game Dev Projects\Tooling-Lab-Template>npm init @eslint/config
Need to install the following packages:
@eslint/create-config@1.4.0
Ok to proceed? (y) y


> sandbox@0.0.1 npx
> create-config

@eslint/create-config: v1.4.0

√ How would you like to use ESLint? · problems
√ What type of modules does your project use? · esm
√ Which framework does your project use? · none
√ Does your project use TypeScript? · javascript
√ Where does your code run? · browser
The config that you've selected requires the following dependencies:

eslint, globals, @eslint/js
√ Would you like to install them now? · No / Yes
√ Which package manager do you want to use? · npm
☕️Installing...

added 2 packages, changed 1 package, and audited 853 packages in 4s

56 packages are looking for funding
  run `npm fund` for details

26 vulnerabilities (17 moderate, 7 high, 2 critical)

To address issues that do not require attention, run:
  npm audit fix

To address all issues (including breaking changes), run:
  npm audit fix --force

Run `npm audit` for details.
Successfully created C:\Users\antd2\Desktop\Game Dev Projects\Tooling-Lab-Template\eslint.config.mjs file.

C:\Users\antd2\Desktop\Game Dev Projects\Tooling-Lab-Template>npm init @eslint/config


 With that being said I created the file manually.  Ater running es lint through the cli I would get this message, 
Even after deleting the eslint.config.mjs file I was still getting this error. 

C:\Users\antd2\Desktop\Game Dev Projects\Tooling-Lab-Template>npx eslint --ext .js resources/scripts
Invalid option '--ext' - perhaps you meant '-c'?
You're using eslint.config.js, some command line flags are no longer available. Please see https://eslint.org/docs/latest/use/command-line-interface for details.

For the second problem I was running into a cli error with the npx webpack command 
It looks like it is looking for a src file or directory but one was not included in the repo and the instructions never mention anything about adding a src directory. 

C:\Users\antd2\Desktop\Game Dev Projects\Tooling-Lab-Template>npx webpack
Entrypoint main =

WARNING in configuration
The 'mode' option has not been set, webpack will fallback to 'production' for this value.
Set 'mode' option to 'development' or 'production' to enable defaults for each environment.
You can also set it to 'none' to disable any default behavior. Learn more: https://webpack.js.org/configuration/mode/

ERROR in main
Module not found: Error: Can't resolve './src' in 'C:\Users\antd2\Desktop\Game Dev Projects\Tooling-Lab-Template'
resolve './src' in 'C:\Users\antd2\Desktop\Game Dev Projects\Tooling-Lab-Template'
  using description file: C:\Users\antd2\Desktop\Game Dev Projects\Tooling-Lab-Template\package.json (relative path: .)
    Field 'browser' doesn't contain a valid alias configuration
    using description file: C:\Users\antd2\Desktop\Game Dev Projects\Tooling-Lab-Template\package.json (relative path: ./src)
      no extension
        Field 'browser' doesn't contain a valid alias configuration
        C:\Users\antd2\Desktop\Game Dev Projects\Tooling-Lab-Template\src doesn't exist
      .js
        Field 'browser' doesn't contain a valid alias configuration
        C:\Users\antd2\Desktop\Game Dev Projects\Tooling-Lab-Template\src.js doesn't exist
      .json
        Field 'browser' doesn't contain a valid alias configuration
        C:\Users\antd2\Desktop\Game Dev Projects\Tooling-Lab-Template\src.json doesn't exist
      .wasm
        Field 'browser' doesn't contain a valid alias configuration
        C:\Users\antd2\Desktop\Game Dev Projects\Tooling-Lab-Template\src.wasm doesn't exist
      as directory
        C:\Users\antd2\Desktop\Game Dev Projects\Tooling-Lab-Template\src doesn't exist

webpack 5.96.1 compiled with 1 error and 1 warning in 146 ms



### How long it took me to finish this?

It took me a 4-5 hours of troubleshooting before I gave up.