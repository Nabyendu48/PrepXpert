# PrepXpert ⭐
This is a Ai generated Mock interview app to help people prepare for their upcoming interviews 

Currently, two official plugins are available:

@vitejs/plugin-react uses Babel for Fast Refresh
@vitejs/plugin-react-swc uses SWC for Fast Refresh
Expanding the ESLint configuration
If you are developing a production application, we recommend updating the configuration to enable type aware lint rules:

Configure the top-level parserOptions property like this:
export default tseslint.config({
  languageOptions: {
    // other options...
    parserOptions: {
      project: ['./tsconfig.node.json', './tsconfig.app.json'],
      tsconfigRootDir: import.meta.dirname,
    },
  },
})
Replace tseslint.configs.recommended to tseslint.configs.recommendedTypeChecked or tseslint.configs.strictTypeChecked
Optionally add ...tseslint.configs.stylisticTypeChecked
Install eslint-plugin-react and update the config:
// eslint.config.js
import react from 'eslint-plugin-react'

export default tseslint.config({
  // Set the react version
  settings: { react: { version: '18.3' } },
  plugins: {
    // Add the react plugin
    react,
  },
  rules: {
    // other rules...
    // Enable its recommended rules
    ...react.configs.recommended.rules,
    ...react.configs['jsx-runtime'].rules,
  },
})
About
No description, website, or topics provided.
Resources
 Readme
 Activity
 Custom properties
Stars
 29 stars
Watchers
 2 watching
Forks
 22 forks
Report repository
Releases
No releases published
Packages
No packages published
Languages
TypeScript
94.8%
 
JavaScript
2.6%
 
CSS
1.8%
 
HTML
0.8%
Footer
