
## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.


## Docker
   [Doc From NextJs](https://nextjs.org/docs/pages/building-your-application/deploying#docker-image)
    

    ```bash
    En el Dockerfile se debe colocar COPY . . para que copie todos los archivos del proyecto, si no los estilos no se aplican.
    En next.config.js se debe colocar el siguiente código para que funcione en docker mejor:
    
    module.exports = {
        output: 'standalone',
    }


    docker build -t nextjs-primero .
    docker container run -dp 3000:3000 nextjs-primero
    docker ps
    docker container stop <container_id>
    ```
