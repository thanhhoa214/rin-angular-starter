# Rin Angular Starter
Angular Starter Template for initialization faster and robust.


### About Me
<img src="https://trello-members.s3.amazonaws.com/59169b4cdb7b86a9f6012efb/e0223ddc9d7e21b236619efc65aa8612/170.png" style="width: 70px; height: 70px; border-radius: 50%;"/>

**Author**: Hòa Nguyễn <br/>
**Phone**: <a href="tel:(+84) 979 210 499">(+84) 979 210 499</a> <br/>
**City**: Ho Chi Minh City, Viet Nam <br/>
**Channels**:
- Linkedin: linkedin.com/in/thanhhoa214/
- Twitter: twitter.com/thanhhoa214
- What'sApp: (+84) 979 210 499

<div style="margin-top: 30px;"></div>

## 1. Branches:

### `RAS-01`: With ESLint + Prettier
All of upcoming libraries install only in development mode. 
```bash
npm install -D LIBRARY_NAME
```
#### ESLint [official document](https://github.com/eslint/eslint): 
TypeScript Linter forces project coding style. Pair with ESLint extension in VSC. 
- `eslint`
- `eslint-plugin-autofix`
- `eslint-plugin-unused-imports`
- `@typescript-eslint/eslint-plugin`
- `@typescript-eslint/parser`
#### Lint-staged [official document](https://github.com/okonet/lint-staged):
Uses with git, lints only unstaged files.
- `lint-staged`
#### Prettier [official document](https://github.com/prettier/prettier): 
Format code. Pair with Prettier extension in VSC. 
- `prettier`
- `pretty-quick`
#### Husky [official document](https://github.com/typicode/husky): 
Supports git hooks (pre-commit). Integrate with `prettier` and `lint-staged` make super power to reduce redundant & "ugly" codes before committing.
- `husky`

### `RAS-02`: With `RAS-01` + NGXS
#### NGXS [official document](https://github.com/ngxs/store): 
State management follows CQRS pattern for Angular application.
- `@ngxs/store`
- `@ngxs/storage-plugin`
- `@ngxs/logger-plugin`
- `immer`
- `@ngxs-labs/immer-adapter` which depends on `immer`
- `ngxs-reset-plugin` for resetting whole store.

### `RAS-03`: With `RAS-01` + Restful API
#### `@openapitools/openapi-generator-cli`
Auto-generate Restful API models & services for using at the hand.
- `@openapitools/openapi-generator-cli` (development only)

### `RAS-04`: With `RAS-01` + GraphQL

#### GraphQL [official document](https://graphql.org/): 
GraphQL provides awesome interactive with Back-end through single endpoint, flexible queries, and so on.
- GraphQL:
  - `graphql`
  - `graphql-tag`
- Apollo:
  - `@apollo/client`
  - `apollo-angular`
  - `apollo-cache-inmemory`
  - `apollo-link-context`
  - `apollo-upload-client` (only if upload file)
- GraphQL Codegen
  - `@graphql-codegen/cli`
  - `@graphql-codegen/import-types-preset`
  - `@graphql-codegen/near-operation-file-preset`
  - `@graphql-codegen/typescript`
  - `@graphql-codegen/typescript-apollo-angular`
  - `@graphql-codegen/typescript-operations` 
- Apollo Config: pair with `Apollo GraphQL` extension in VSC


### `RAS-05`: With `RAS-01` + Multilingual
#### Ngx Translate:
- `@ngx-translate/core`
- `@ngx-translate/http-loader`

### `RAS-06`: With `RAS-01` + Ionic(Capacitor)+
#### Ionic [official document](https://ionicframework.com/): 
Great hybrid framework for building mobile application by web technologies, provides awesome **UI Components** and **Native Plugins**.
- Ionic
  - `@ionic/angular`
  - `@ionic/angular-toolkit` (development only)
  - `@ionic-native/core`
  - `@ionic-native/splash-screen`
- Capacitor: Building iOS/Android/Electron native apps while using web build package...
  - `@capacitor/core`
  - `@capacitor/android`
  - `@capacitor/ios`
  - `@capacitor/cli` (development only)
- `cordova-res`: Autogenerate splashscreen + icon for iOS and Android, still has a small issue on Android with fix [Create app icons](https://developer.android.com/studio/write/image-asset-studio#access)
- `jetifier` to migrate all Java/Kotlin packages to Android X.

### `RAS-07`: With `RAS-02` + `RAS-03`

### `RAS-08`: With `RAS-02` + `RAS-04`

### `RAS-09`: With `RAS-02` + `RAS-03` + `RAS-05`

### `RAS-10`: With `RAS-02` + `RAS-04` + `RAS-05`

### `RAS-11`: With `RAS-02` + `RAS-03` + `RAS-06`

### `RAS-12`: With `RAS-02` + `RAS-04` + `RAS-06`

### `RAS-13`: With `RAS-02` + `RAS-03` + `RAS-05` + `RAS-06`

### `RAS-14`: With `RAS-02` + `RAS-04` + `RAS-05` + `RAS-06`

### `RAS-15`: With `RAS-01` + Gitlab Mobile CI/CD

## 2. Awesome libraries for solving special problems:
### 1. CryptoJS [offical document](https://cryptojs.gitbook.io/docs/)
Especial use for encrypt/decrypt mechanism.
- `crypto-js`
- `@types/crypto-js`

### 2. ngx-timeago [offical document](https://github.com/ihym/ngx-timeago)
Chatting app with timeago like FB comment records.
- `ngx-timeago`

### 3. ngx-mask [offical document](https://github.com/JsDaddy/ngx-mask)
When creating mask for input.
- `ngx-mask` 

### 4. cli-typescript-class-organizer
Organize your typescript class (can be integrated with pre-commit above)
- `cli-typescript-class-organizer`


## 3. Capacitor Native Plugins:
- Official Plugins: https://capacitorjs.com/docs/apis/
- Ionic Native Plugins: https://ionicframework.com/docs/native/
  - BranchIO: Super URL Scheme, for sharing your internal information with others (either has an app or not).
  - Facebook login: `@capacitor-community/facebook-login`
- My Plugins: 
  - [`zalo-auth-capacitor-plugin`](https://www.npmjs.com/package/zalo-auth-capacitor-plugin): Login/logout, message, or sharing with Zalo (supports iOS/Android)
