# eslint-prettier-config
Setup steps and resources for configuring eslint and prettier.

## Resources 
* https://blog.echobind.com/integrating-prettier-eslint-airbnb-style-guide-in-vscode-47f07b5d7d6a
* https://www.youtube.com/watch?v=YIvjKId9m2c

## Steps 
* npm packages
```
npm install -D eslint prettier 
npx install-peerdeps --dev eslint-config-airbnb
npm install -D eslint-config-prettier eslint-plugin-prettier
```
* for projects using babel to transform javascript, you likely need to include the babel-eslint package
``` 
npm install -D babel-eslint
```
* editor settings...


## Troubleshooting
* in some cases (perhaps depending on how babel is used), eslint may throw incorrect parsing errors
    - unable to parse '='
    - potential fix:  use 'babel-eslint' parser
        + https://stackoverflow.com/questions/36001552/eslint-parsing-error-unexpected-token

        
