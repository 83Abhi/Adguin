# Adguin
## Features
- ⚡️ Next.js 12
- ⚛️ React 18
- 📝 Tailwind CSS
- ⛑ TypeScript
- ✨ Styled Components - CssInJs for component styling
- 📏 ESLint — To find and fix problems in your code
- 💖 Prettier — Code Formatter for consistent style
- 🐶 Husky — For running scripts before committing
- 🚓 Commitlint — To make sure your commit messages follow the convention
- 🚫 lint-staged — Run ESLint and Prettier against staged Git files
- ⚙️ EditorConfig - Consistent coding styles across editors and IDEs
- 🗂 Path Mapping — Import components or images using the `~/` prefix
- ‽ Either Error Handler - For error handling. (Either is designed to hold either a left or a right value but never both).


## Quick Start

The best way to start with this template is using [Create Next App](https://nextjs.org/docs/api-reference/create-next-app).

```
# yarn
yarn create next-app -e https://github.com/yazaldefilimonepinto/clean-arch-nextjs-starter
# npm
npx create-next-app -e https://github.com/yazaldefilimonepinto/clean-arch-nextjs-starter
```

### Development

To start the project locally, run:

```bash
  npm dev
  our
  yarn dev
```

Open `http://localhost:3000` with your browser to see the result.


### Requirements

- Node.js >= 12.22.0
- npm our yarn

### Directory Structure

- [`.husky`](.husky) — Husky configuration and hooks.<br>
- [`public`](./public) — Static assets such as robots.txt, images, and favicon.<br>
- [`src`](./src) — Application source code, including pages, components, styles.<br>

### Scripts
- `yarn/npm dev` — Starts the application in development mode at `http://localhost:3000`.
- `yarn/npm build` — Creates an optimized production build of your application.
- `yarn/npm start` — Starts the application in production mode.
- `yarn/npm lint` — Runs ESLint for all files in the `src` directory.


Folder Structure Conventions
============================

> Folder structure options and naming conventions for software projects

### A typical top-level directory layout

    .
    ├── husky                   
    ├── vscode                   
    ├── src 
    ├── public
    ├── babelrc                    
    ├── editorconfig                   
    ├── prettierrc
    ├── jest.config.ts
    ├── next-env.d.ts
    ├── package.json
    ├── gitignore
    ├── yarn.lock
    ├── tsconfig.json
    └── README.md
    
    

> Use short lowercase names at least for the top-level files and folders except
> `LICENSE`, `README.md`


### Husky Files

    .
    ├── ...
    ├── husky                   
    │   ├── pre-commit                             
    └── ...
    
    
- Husky can be used to automate tasks that need to be run before committing code to the repository, such as linting and formatting code.

- Husky can be configured in a Next.js application by adding a "husky" section to the package.json file. Within this section, developers can specify the scripts that should be run as pre-commit hooks.

### src Files

    .
        ├── ...
        ├── src                   
        │   ├── application  
        │   │         ├── protocols/services
        │   │         │         ├──Iinfo-storage.ts
        │   │         │         └──index.ts
        │   │         │                       
        │   │         └── usecases
        │   │                   ├── index.ts
        │   │                   └── info-usecase.ts
        │   │
        │   ├── domain   
        │   │         ├──entities
        │   │         │         ├──Info.ts
        │   │         │         ├──index.ts 
        │   │         └── usecases
        │   │                   ├── Iinfo-usecase.ts
        │   │                   └──index.ts
        │   │                 
        │   │          
        │   │          
        │   ├── infrastructure
        │   |         └── factories
        │   |                   ├──info-factory.ts
        │   |                   └──index.ts
        │   |                       
        │   |         
        │   |         
        │   ├── pages
        │   |         ├──_app.tsx
        │   |         ├──_document.tsx
        │   |         └──index.tsx
        │   |       
        │   |       
        │   |       
        │   └── shared
        │             ├──settings
        │             │        ├──jest-setup.ts
        │             ├──styles
        │             │        ├──globals.ts
        │             └──either
        │                      └──index.ts
        │           
        │           
        └── ...
        
#### src structure
- The application layer typically contains components that handle user interactions and perform operations such as fetching data from APIs, manipulating the data, and rendering it to the user interface. In the context of a Next.js application, this layer can include pages, components, and utility functions like Server-side rendering, dynamic imports, routing and api routes.

- Domain layer can include domain entities, domain services, and any business rules or logic that are specific to the application.

- The infrastructure layer holds the architecture and all UI components of the project with different templates.

- All the new pages will be automatically route on the Pages section, which holds all the exported components and render it on the screen.

- The Shared layer is responsible for providing a set of common components and utilities that can be used throughout the application, regardless of the specific use case. Such as data access components, and utility functions.
        
    
### Public Files

    .
        ├── ...
        ├── Pubic                   
        │   ├── favicon.ico          
        │   ├── vercel.svg            
        └── ...

- Public section will hold all the static files, logos, svgs, pngs and all is available publically to the users.

 ### vscode Files 
 
     .
        ├── ...
        ├── Pubic                   
        │   ├── settings.json            #add husk and lint-staged
        │               
        └── ...
    
 


