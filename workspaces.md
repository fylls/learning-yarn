<div align="center">

[![](https://yt-embed.herokuapp.com/embed?v=G8KXFWftCg0)](https://www.youtube.com/watch?v=G8KXFWftCg0)

# Yarn Workspaces

</div>

`monorepo method`

babel and react

instead of separating packages out and two different repos and two basically different folder structures, what about putting everything into one?

**Why?** you can share dependencies and code between the packages

`package.json`

```json
{
  "private": true,
  "worspaces": ["client", "server"]
}
```
