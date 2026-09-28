<div align="center">

<img src="https://capsule-render.vercel.app/api?type=venom&color=0:0d1117,50:1f2a44,100:714B67&height=230&section=header&text=SAMI%20ULLAH%20KHATTAK&fontSize=46&fontColor=58a6ff&animation=fadeIn&fontAlignY=38&desc=Odoo%20Developer%20%7C%20ERP%20Engineer%20%7C%20DevOps&descSize=16&descAlignY=60&descColor=c9d1d9" width="100%" alt="Sami Ullah Khattak Header"/>

<a href="https://git.io/typing-svg">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=19&duration=3000&pause=1000&color=58A6FF&center=true&vCenter=true&repeat=true&width=750&height=45&lines=Odoo+Developer+%7C+ERP+Module+Development;Python+%7C+PostgreSQL+%7C+Docker;Odoo+Server+Deployment+%26+Configuration;Automating+Business+Workflows+with+Odoo;React+%7C+React+Native+%7C+TypeScript" alt="Typing Header" />
</a>

<br/>

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/sami-ullah-khattak-3a400625a/)
[![Upwork](https://img.shields.io/badge/Upwork-6FDA44?style=for-the-badge&logo=upwork&logoColor=white)](https://www.upwork.com)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:samiulahktk@gmail.com)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://instagram.com/samiiktk)
[![Facebook](https://img.shields.io/badge/Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white)](https://www.facebook.com/04467565kjhj/)

![Profile Views](https://komarev.com/ghpvc/?username=Sami-Ullah-Khattak&style=flat-square&color=714B67&label=PROFILE+VIEWS)
![Followers](https://img.shields.io/github/followers/Sami-Ullah-Khattak?style=flat-square&color=58a6ff&labelColor=0d1117)
![Repos](https://img.shields.io/badge/Open_to-Odoo_Projects-714B67?style=flat-square&labelColor=0d1117)
![Location](https://img.shields.io/badge/Islamabad-Pakistan_🇵🇰-01411C?style=flat-square&labelColor=0d1117)

</div>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

## 👨‍💻 About Me

```python
class SamiUllahKhattak:
    role       = "Software Engineer @ eAlam Group"
    location   = "Islamabad, Pakistan 🇵🇰"
    experience = "3+ years building production web & mobile apps"

    focus      = ["Odoo ERP", "QWeb Reports", "Custom Workflows", "Docker Deployments"]
    also_builds = ["React", "React Native", "TypeScript", "Flask APIs"]

    philosophy = "Clean code. Solid UX. Systems that scale."

    def journey(self):
        return "HTML/CSS → React → Odoo → Dockerized ERPs 🐳"
```

Started as a UI developer, grew into application architecture. Today I build **Odoo modules, QWeb reports, and automated business workflows**, and I deploy them with Docker.

<br/>

<table>
<tr>
<td width="50%" valign="top">

### 🔭 Current Status

| | |
|---|---|
| 🛠️ **Working on** | Odoo modules & custom QWeb views |
| 📖 **Learning** | Odoo ORM, wizards, report generation |
| 🤝 **Open to** | Odoo & ERP collaborations |
| 🆘 **Need help with** | Advanced QWeb templating |
| 💬 **Ask me about** | ERP, React / React Native, UI architecture |
| ⚡ **Fun fact** | Started with HTML/CSS, ended up containerizing ERPs |

</td>
<td width="50%" valign="top">

### 🎯 2026 Goals

- [x] Ship production Odoo modules
- [x] Containerize Odoo with Docker Compose
- [ ] Master QWeb & custom PDF reports
- [ ] Publish open-source Odoo addons
- [ ] Finish B.Sc. Computer Science
- [ ] Write technical posts on ERP dev

</td>
</tr>
</table>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

## 🧰 Tech Stack

<div align="center">

**Frontend**<br/>
<img src="https://skillicons.dev/icons?i=react,ts,js,html,css,sass,bootstrap&theme=dark" /><br/>
<sub>React · TypeScript · JavaScript · HTML5 · CSS3 · Sass · Bootstrap &nbsp;|&nbsp; React Native for mobile</sub>

<br/><br/>

**Backend & Data**<br/>
<img src="https://skillicons.dev/icons?i=python,flask,postgres&theme=dark" />
<img src="https://img.shields.io/badge/Odoo-714B67?style=for-the-badge&logo=odoo&logoColor=white" height="48"/><br/>
<sub>Python · Flask · PostgreSQL · Odoo (ORM, QWeb, wizards, reports)</sub>

<br/><br/>

**DevOps & Tools**<br/>
<img src="https://skillicons.dev/icons?i=docker,git,github,linux,nginx,postman,vscode&theme=dark" /><br/>
<sub>Docker · Docker Compose · Git · GitHub · Linux · Nginx · Postman · VS Code</sub>

</div>

<br/>

### 📊 Skill Focus

```mermaid
pie showData title Where my time goes
    "Odoo / Python" : 40
    "React / React Native" : 30
    "Docker / DevOps" : 15
    "PostgreSQL" : 10
    "UI / UX" : 5
```

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

## 🧪 Code I Enjoy Writing

A small Odoo model with a computed field and a workflow action, the kind of thing I build every day:

```python
from odoo import models, fields, api


class SaleApproval(models.Model):
    _name = "sale.approval"
    _description = "Sale Approval Request"
    _inherit = ["mail.thread"]

    name = fields.Char(required=True, tracking=True)
    amount = fields.Monetary(currency_field="currency_id")
    currency_id = fields.Many2one("res.currency", default=lambda s: s.env.company.currency_id)
    state = fields.Selection(
        [("draft", "Draft"), ("review", "In Review"), ("approved", "Approved")],
        default="draft", tracking=True,
    )
    is_high_value = fields.Boolean(compute="_compute_high_value", store=True)

    @api.depends("amount")
    def _compute_high_value(self):
        for rec in self:
            rec.is_high_value = rec.amount > 10000

    def action_submit(self):
        self.write({"state": "review"})
        self.message_post(body="Submitted for approval 🚀")
```

And the deployment side:

```yaml
# docker-compose.yml
services:
  odoo:
    image: odoo:20
    depends_on: [db]
    ports: 127.0.0.1:${ODOO_EXT_PORT}:8069"
    volumes:
      - ./addons:/mnt/extra-addons
      - odoo-data:/var/lib/odoo
  db:
    image: postgres:18
    env_file:
      - .env
    environment:
      POSTGRES_DB: ${POSTGRES_DB}
      POSTGRES_USER: ${POSTGRES_USER}
      POSTGRES_PASSWORD: ${POSTGRES_PASSWORD}
volumes:
  odoo-data:
```

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

## 💼 Experience

```mermaid
timeline
    title Career Timeline
    Intern @ eAlam Group : HTML / CSS / JS : LESS, SASS : Databases
    Junior Software Engineer @ eAlam Group : Web development : Git workflows : Team collaboration
    Software Engineer @ eAlam Group : React Native · ReactJS · TypeScript : PostgreSQL · Docker · Odoo
```

| Period | Role | Company | Stack |
|:--|:--|:--|:--|
| **2 yrs 7 mos** *(current)* | Software Engineer | **eAlam Group** | React Native · ReactJS · TypeScript · PostgreSQL · Docker · Odoo |
| 6 mos | Junior Software Engineer | eAlam Group | Web development · Git workflows · Team collaboration |
| 8 mos | Intern | eAlam Group | HTML/CSS/JS · LESS · SASS · Databases |
| **4 yrs** *(ongoing)* | UI Developer (Freelance) | **Upwork** | React.js · JavaScript · UI/UX for diverse clients |
| 6 mos | Computer Programmer | IMMS | React.js · React Native |

## 🎓 Education

| | |
|:--|:--|
| 📚 **B.Sc. Computer Science** *(in progress)* | Alhamd Islamic University, Islamabad · Nov 2023 – Feb 2027 · C++, OOP, Data Structures |
| 🎓 **Pre-Medical** · Grade A | Ummah Children Academy · 2011 – 2022 |

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

## 📈 GitHub Stats

<div align="center">

<img height="180" src="https://github-readme-stats.vercel.app/api?username=Sami-Ullah-Khattak&show_icons=true&theme=tokyonight&hide_border=true&include_all_commits=true&count_private=true&rank_icon=github" />
<img height="180" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Sami-Ullah-Khattak&theme=tokyonight&hide_border=true&layout=compact&langs_count=8" />

<img src="https://streak-stats.demolab.com/?user=Sami-Ullah-Khattak&theme=tokyonight&hide_border=true" />

<img src="https://github-readme-activity-graph.vercel.app/graph?username=Sami-Ullah-Khattak&theme=tokyo-night&hide_border=true&area=true&custom_title=Contribution%20Activity" width="100%" />

</div>

### 🐍 Contribution Snake

<div align="center">
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Sami-Ullah-Khattak/Sami-Ullah-Khattak/output/github-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Sami-Ullah-Khattak/Sami-Ullah-Khattak/output/github-snake.svg" />
  <img alt="Contribution snake" src="https://raw.githubusercontent.com/Sami-Ullah-Khattak/Sami-Ullah-Khattak/output/github-snake-dark.svg" />
</picture>
</div>

### 🏆 Trophies

<div align="center">

![Trophies](https://github-profile-trophy.vercel.app/?username=Sami-Ullah-Khattak&theme=tokyonight&no-frame=true&no-bg=true&margin-w=6&column=7)

</div>

<img src="https://user-images.githubusercontent.com/73097560/115834477-dbab4500-a447-11eb-908a-139a6edaec5c.gif" width="100%">

## 💡 Dev Wisdom

<div align="center">

![Dev Quote](https://quotes-github-readme.vercel.app/api?type=horizontal&theme=tokyonight)

</div>

## 🤝 Let's Work Together

> 💬 Reach out if you're working on **Odoo / ERP**, need a **React or React Native** developer, or want to collaborate on something interesting.

<div align="center">

| 🧩 Odoo Module Development | 📄 QWeb & PDF Reports | 🐳 Docker Deployments | 📱 React Native Apps |
|:--:|:--:|:--:|:--:|
| Custom apps, workflows, automation | Invoices, labels, custom layouts | Odoo + PostgreSQL + Nginx setups | Cross-platform mobile UIs |

<br/>

[![Let's Connect](https://img.shields.io/badge/Let's_Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/sami-ullah-khattak-3a400625a/)
[![Send Email](https://img.shields.io/badge/Send_Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:samiulahktk@gmail.com)
[![Hire on Upwork](https://img.shields.io/badge/Hire_on_Upwork-6FDA44?style=for-the-badge&logo=upwork&logoColor=white)](https://www.upwork.com)

</div>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0d1117,50:1f2a44,100:714B67&height=120&section=footer" width="100%"/>

<div align="center">
<sub>Built with precision · Islamabad, Pakistan 🇵🇰</sub>
</div>
