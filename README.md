# Tailwind CSS plugin for Fresh

A Tailwind CSS plugin to use in Fresh.

```ts
// dev.ts
import { Builder } from "fresh/dev";
import { app } from "./main.ts";
import { tailwind } from "@fresh/plugin-tailwind";

const builder = new Builder();
await tailwind(builder, app);

if (Deno.args.includes("build")) {
  await builder.build(app);
} else {
  await builder.listen(app);
}
```

To learn more about Fresh go to
[https://fresh.deno.dev/](https://fresh.deno.dev/).
