<h1 align="center">Angular Boilerplate</h1>

<p align="center">
  <img src="https://img.icons8.com/ios-filled/150/000000/angularjs.png" alt="angular-logo" width="120px" height="120px"/>
  <br>
  <i>Angular starter for enterprise-grade front-end projects, built under a clean architecture 
    <br> that helps to scale and maintain a fast workflow.</i>
  <br>
</p>

<p align="center">
  <a href="https://angularboilerplate.vercel.app"><strong>https://angularboilerplate.vercel.app</strong></a>
  <br>
</p>

<p align="center">
  <a href="CONTRIBUTING.md">Contributing Guidelines</a>
  ยท
  <a href="https://github.com/juanmesa2097/angular-boilerplate/issues">Submit an Issue</a>
  <br>
  <br>
</p>
<hr>

## โ๏ธ Features

- Strict mode.
- Lazy loading.
- Smart and pure components pattern.
- SCAM pattern.
- Self-contained components and encapsulated modules.
- Components types (e.g. component, page).
- Amazing directory structure.
- PWA
- Dynamic titles and content meta tags.
- TailwindCSS.
- Dark mode and theme configuration.
- Scalable CSS architecture in favor of TailwindCSS layers.
- [Lighthouse](https://developers.google.com/web/tools/lighthouse) reports improved.
- ESLint.
- Run unit tests & lint code using [Husky](https://github.com/typicode/husky) & validate commit messages using [commitlint](https://github.com/conventional-changelog/commitlint)

## ๐ Pages

- General
  - home
  - not-found
- Auth
  - sign-in
  - sign-up
  - forgot-password
  - forgot-password-email-sent
  - password-reset
  - password-reset-succeeded
  - password-reset-failed
- Settings
  - account
  - appearance
  - billing
  - blocked-Users
  - notifications
  - security
  - security-log
- User
  - my-profile
  - overview
- Features
  - dashboard

## ๐งฑ Self-contained components

- footer
- header
- layout

## ๐ก Services

- AuthService
- SeoService
- ThemeService

## ๐ Custom directives

- click-outside: detects when the user clicks outside an element.

## ๐งช Custom pipes

- bytes: transforms a numeric value into bytes, KB, MB, GB, etc.

## ๐?๏ธ Make some initial tweaks

- Change pages routes:

  Go to `src/app/core/utils/router.utils.ts` to find all the registered routes inside a config object.

  For example, you could replace `sign-in` with `SignIn`, `login` or `iniciar_sesion`

- Change your TailwindCSS configuration:

  You can find the config file in the project root, then you can refer to https://tailwindcss.com/docs/configuration to learn how to make your own adjustments.

- Set a default theme (First time load)

  Go to `src\app\@core\services\theme\theme.config.ts` and change the following line of code

  from operating system preference

  ```ts
  export const DEFAULT_BASE_THEME = ThemeList.System;
  ```

  to light mode

  ```ts
  export const DEFAULT_BASE_THEME = ThemeList.Light;
  ```

  or dark mode

  ```ts
  export const DEFAULT_BASE_THEME = ThemeList.Dark;
  ```

## โฉ๏ธ Project structure

```console
โโโโapp
โ   โโโโ@core
โ   โ   โโโโdirectives
โ   โ   โ   โโโโclick-outside
โ   โ   โโโโguards
โ   โ   โโโโinterceptors
โ   โ   โโโโpipes
โ   โ   โ   โโโโbytes
โ   โ   โโโโservices
โ   โ   โ   โโโโseo
โ   โ   โ   โโโโtheme
โ   โ   โโโโutils
โ   โโโโ@shell
โ   โ   โโโโft
โ   โ   โโโโui (layout components)
โ   โ       โโโโfooter
โ   โ       โโโโheader
โ   โ       โโโโlayout
โ   โ       โโโโnot-found
โ   โโโโcomponents (generic shared components)
โ   โโโโpages
โ       โโโโauth
โ       โ   โโโโpages
โ       โ   โ   โโโโforgot-password
โ       โ   โ   โโโโforgot-password-email-sent
โ       โ   โ   โโโโpassword-reset
โ       โ   โ   โโโโpassword-reset-failed
โ       โ   โ   โโโโpassword-reset-succeeded
โ       โ   โ   โโโโsign-in
โ       โ   โ   โโโโsign-up
โ       โ   โโโโservices
โ       โโโโdashboard
โ       โโโโhome
โ       โโโโsettings
โ       โ   โโโโpages
โ       โ       โโโโaccount
โ       โ       โโโโappearance
โ       โ       โโโโbilling
โ       โ       โโโโblocked-users
โ       โ       โโโโnotifications
โ       โ       โโโโsecurity
โ       โ       โโโโsecurity-log
โ       โโโโuser
โ           โโโโpages
โ               โโโโmy-profile
โ               โโโโoverview
โโโโassets
โโโโenvironments
โโโโtheme
    โโโโ01-base
    โโโโ02-components
    โโโโ03-utilities
```

## ๐งโโ๏ธ Commands

| Command | Description                      | NPM           | Yarn       | Pnpm       | Background command                           |
| ------- | -------------------------------- | ------------- | ---------- | ---------- | -------------------------------------------- |
| ng      | See available commands           | npm run ng    | yarn ng    | pnpm ng    | ng                                           |
| start   | Run your app in development mode | npm start     | yarn start | pnpm start | ng serve                                     |
| build   | Build your app for production    | npm run build | yarn build | pnpm build | ng build                                     |
| watch   | Run build when files change.     | npm run watch | yarn watch | pnpm watch | ng build --watch --configuration development |
| test    | Run your unit tests              | npm run test  | yarn test  | pnpm test  | ng test                                      |
| lint    | Use ESLint to lint your app      | npm run lint  | yarn lint  | pnpm lint  | ng lint                                      |
