# zanahorio-skills
一个存放我个人喜欢用的 skills 的仓库，一切为了 AI Agent！


# Claude Code 代码改动配置说明
对于 Claude Code 来说，配置 plugins 的方式很简单：
1. 首先在技能文件夹里面增加一个 `.claude-plugin` 文件夹，然后在里面加上两个文件，分别是
  - `marketplace.json`，里面记录一下这个插件模块的名称和作者:
      ```JSON
      {
         "name": "Doreamon",
         "owner": { "name": "ZanahorioJose" },
         "plugins": [{ "name": "Doreamon", "source": "./" }]
      }
      ```
  - `plugin.json`，里面记录一下这些技能的文件位置：  
      ```JSON
      {
         "name": "Doreamon",
         "skills": "./<Claude Code 文件夹技能位置>/"
      }
      ```
2. 启动 Claude Code，在 Claude Code 里面注册技能。
