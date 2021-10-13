# 1st step => yarn run eslint --init

use any popular rules
yarn add prettier eslint-config-prettier --dev
extends prettier
set any rules value with its appropriate property
for prettier create .prettierrc (all rules here) file and .prettierignore file
"lint:fix": "npx eslint . --ext .js,.ts,.tsx --fix" add this in script

## step 2 => npx mrm@2 lint-staged

this will automatically install husky and list staged for auto linting before
commit any changes change config in packages.json like this:
"lint-staged": {
"_..{js,ts,tsx}": "npx eslint . --ext .js,.ts,.tsx --fix",
"_.{js,ts,tsx,css,md}": "npx prettier --write"
}

<!-- "lint-staged": {
    "*{.tsx,.ts}": "npx eslint '**/*{.ts,.tsx}' --fix",
    "*.{ts,tsx,css,md}": "npx prettier --write"
  } -->

## step 3 => yarn add react-bootstrap bootstrap react-icon node-sass

1. sass setup
   setup all sass variable, global, file
   override bootstrap
2. setup relative path for import file absolutely in tsconfig.json => "baseUrl": "./src"
   -----in component/common folder-----
3. building header: add navbar and set react icon
4. banner: building carousel and list group
5. product: card
   -----in home component/folder-----
6. products section

## step 4 => yarn add axios

1. create .env.local file in the root => REACT_APP_BASE= http: //localhost:8000
2. services/httpService.ts => axios instance
3. services/productService.ts
4. services/storeService.ts
5. types.d.ts =>schemas
6. pages/home

## custom hooks

1. utils/imageParser.ts for optimizing images
2. hooks/useAsync.ts for fetching data
3. component/home
4. react skeleton
5. pages/productDetails/ProductDetails.tsx

## redux(core) and typescript

1. redux/ folder
2. all about redux core
3. component/home
4. component/home/pageDetails.tsx
5. Redux/action => actionCreators
6. types.ts => all data type definition
7. services/authServices.ts

## advance redux

1. redux thunk
2. Redux/store.ts
3. AuthReducer.ts
4. component/forms
5. npm i redux-persistance => data persisting
6. store
7. services/httpServices.ts => interceptors

## react core ui => admin template

1. merge both package.json
2. create admin folder to pull all template code
3. merchant Dashboard

## performance optimization

1. using useMemo, useCallback, memo
2. react profiler
3. .env.local => GENERATE_SOURCEMAP = false => to avoid source .map file in production

## node js backend
