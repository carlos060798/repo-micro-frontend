# Notas de microfrontend  para el curso de microfrontend

- cracion d eproyectos de reac  comnado  npm create  mf-app 
# exposicion de los microfrontend

para exponer los componntes dentro de un microfrontend se debe de exportar los componentes en el

se debe configurar en el archivo de  webpack.config.js

 new ModuleFederationPlugin({
      name: "navbar", // nombre del modulo del archivo de webpack
      filename: "remoteEntry.js",
      remotes: {}, // para configurar el archivo  importaciones desde otros webpack 
      exposes: { // para exponer los componentes
        "./Navbar": "./src/componets/Navbar.jsx", // se debe de poner la ruta del componente con un identificador 
        //
      },
 )}