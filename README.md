# Nuxt memory leak minimal reproduction
Refering to [this](https://github.com/oven-sh/bun/issues/14389) bun issue.
## reproduction
this memory leak occurs on bun version 1.1.29

`docker build -t memoryLeak .`
and 
`docker run -p 3000:3000 memoryLeak`

## debugging
you can run `bun run preview:debug:bun` and you will see in console for inspection.
