<h1 align="center">Team 5401 Team Wiki</h1> 

<p align="center">Made with ♥ by <a href="https://zeon.studio/"> Zeon Studio</a> & Lain & Jared</p>

### Purpose

This is a website that will host documentation for FIRST Robotics Team 5401.  Sub-teams such as Business, CADD, Programming, and even Scouting have their documentation pages that are searchable via the searchbar.

### 📦 Tech Stack

- [Hugo](https://gohugo.io/)
- [Tailwind CSS](https://tailwindcss.com/)
- [PostCSS](https://postcss.org/)
- [PurgeCSS](https://purgecss.com/)
- [AutoPrefixer](https://autoprefixer.github.io/)
- [Hugo Modules](https://gohugo.io/hugo-modules/) by [Gethugothemes](https://gethugothemes.com/hugo-modules)
- [Markdown](https://markdownguide.org/)
- [Prettier](https://prettier.io/)
- [Jshint](https://jshint.com/)
- [Github Actions](https://github.com/features/actions)

---

### ⚙️ Prerequisites

To start using this template, you need to have some prerequisites installed on your machine.

- [Hugo Extended v0.115+](https://gohugo.io/installation/)
- [Node v18+](https://nodejs.org/en/download/)
- [Go v1.20+](https://go.dev/doc/install)

### 👉 Project Setup

We build this custom script to make your project setup easier. It will create a new Hugo theme folder, and clone the Hugoplate theme into it. Then move the exampleSite folder into the root directory. So that you can start your Hugo server without going into the exampleSite folder. Use the following command to setup your project.

```bash
npm run project-setup
```

### 👉 Install Dependencies

Install all the dependencies using the following command.

```bash
npm install
```

### 👉 Development Command

Start the development server using the following command.

```bash
npm run dev
```

### 🎬 Still Confused? Watch a Quick Video

https://github.com/zeon-studio/hugoplate/assets/58769763/c260c0ae-91be-42ce-b8db-aa7f11f777bd

### 👉 Social Links

You can change the social links from the `data/social.json` file. Add your social links here, and they will automatically be displayed on the site.

---

## 🛠 Advanced Usage

We have added some custom scripts to make your life easier. You can use these scripts to help you with your development.

### 👉 Update Theme

If you want to update the theme, then you can use the following command. It will update the theme to the latest version.

```bash
npm run update-theme
```

> **Note:** This command will work after running `project-setup` script.

### 👉 Update Modules

We have added a lot of modules to this template. You can update all the modules using the following command.

```bash
npm run update-modules
```

### 👉 Remove Dark Mode

If you want to remove dark mode from your project, then you have to do it manually from everywhere. So we build a custom script to do it for you. you can use the following command to remove dark mode from your project.

```bash
npm run remove-darkmode
```

> **Note:** This command will work before running `project-setup` script. If you already run the `project-setup` command, then you have to run `npm run theme-setup` first, and then you can run this command. afterward, you can run `npm run project-setup` again.

---

## 🚀 Build And Deploy

After you finish your development, you can build or deploy your project almost everywhere. Let's see the process:

### 👉 Build Command

To build your project locally, you can use the following command. It will purge all the unused CSS and minify all the files.

```bash
npm run build
```

### 👉 Deploy Site

- [Github Actions](https://github.com/features/actions)


And if you want to Host some other hosting platforms. then you can build your project, and you will get a `public` folder. that you can copy and paste on your hosting platform.

> **Note:** You must change the `baseURL` in the `hugo.toml` file. Otherwise, your site will not work properly.

---

## 🔒 Guide to Staying Compliant

### 📝 License

Copyright (c) 2023 - Present, Designed & Developed by [Zeon Studio](https://zeon.studio/)

**Code License:** Released under the [MIT](https://github.com/zeon-studio/hugoplate/blob/main/LICENSE) license.

