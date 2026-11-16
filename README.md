
[![My Skills](https://skillicons.dev/icons?i=python,html,css,js,go,arduino,linkedin,kali,git,discord,instagram)](https://skillicons.dev)

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
