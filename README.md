```js
module.exports = class Me {
  constructor(obj = {}) {
    for (const prop in obj) {
      this[prop] = obj[prop];
    }
  }

  static getKnownTechnologies() {
    return {
      Languages: ["Javascript", "NodeJS"],
      Frameworks: ["ExpressJS", "GraphQL"],
      Softwares: {
        inProgress: ["Docker", "Kubernetes", "AWS", "Azure"],
        Known: ["Sqitch", "PGAdmin4"],
        Databases: ["PostgreSQL", "Redis", "MongoDB"],
      },
    };
  }

  static getGoalsToCome() {
    const certifications = [
      "AWS Certified Cloud Practitioner",
      "Microsoft Certified: Azure Fundamentals",
      "AWS Certified Solutions Architect – Associate",
      "Microsoft Certified: Azure Solutions Architect Expert",
    ];
    return `Get multiple certifications ${certifications} for the purposes of becoming an accomplished DevOPS.`;
  }
};
```

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=MrSnakeDoc&layout=compact&langs_count=6&theme=github_dark)
![MrSnakeDoc GitHub stats](https://github-readme-stats.vercel.app/api?username=MrSnakeDoc&show_icons=true&theme=github_dark)

[![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=MrSnakeDoc&repo=oparadis&theme=github_dark)](https://github.com/MrSnakeDoc/oparadis)
[![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=MrSnakeDoc&repo=Tinierurl&theme=github_dark)](https://github.com/MrSnakeDoc/Tinierurl)
[![Readme Card](https://github-readme-stats.vercel.app/api/pin/?username=MrSnakeDoc&repo=weather-app&theme=github_dark)](https://github.com/MrSnakeDoc/weather-app)
