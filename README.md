- 👁️ My name is Harlon Hutchison.
- 👀 I’m interested in programming, leadership, credit, and business intelligence ...
- ⚡ Fun fact: ... I enjoy data-driven projects!
[![My Skills](https://skillicons.dev/icons?i=python,html,css,js,go,arduino,linkedin,linux,kali)](https://skillicons.dev)

import { generateSnakeAnimation } from "generate-snake-animation";

const outputs = [
  {
    format: "svg",
    drawOptions: {
      // ..
    },
  },
];

const results = await generateSnakeAnimation(
  {
    platform: "github", // supports github, gitlab and forgejo (codeberg)
    username: "platane",
    githubToken: process.env.GITHUB_TOKEN,
  },
  outputs,
);

fs.writeFileSync("snake.svg", results[0]);
