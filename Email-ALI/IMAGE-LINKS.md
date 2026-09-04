# Email image links (SharePoint/OneDrive direct URLs)

Fill in the **Direct URL** column for each image, then send this file back and
the email template + Power Automate lookup will be wired to these URLs.

## How to get each Direct URL
1. In OneDrive (web), right-click the image → **Share**.
2. Set permission to **"People in CenterPoint Energy with the link"** (Anyone is usually blocked on the CNP tenant).
3. Click **Copy link** — you'll get something like
   `https://cnp-my.sharepoint.com/:i:/g/personal/first_last_cnp_com/EaBc123?e=abcd`
4. **Append `&download=1`** to the end (use `?download=1` if the link has no `?`).
   That returns the raw image so `<img src>` can render it.
   Final: `https://cnp-my.sharepoint.com/:i:/g/personal/first_last_cnp_com/EaBc123?e=abcd&download=1`

> Reliability note: these load only for CenterPoint recipients, and Outlook desktop
> may still show a broken image until the user clicks "Download pictures." Firebase
> hosting avoids this if you change your mind.

---

## 1. Persona hero banner  (600×180, top of email)  — 1 per persona
| Persona id       | File                                 | Direct URL |
|------------------|--------------------------------------|------------|
| ai_pioneer       | Persona/Banner/Ai-Pioneer.png        |            |
| domain_specialist| Persona/Banner/Domain-Specialist.png |            |
| emerging_adopter | Persona/Banner/Emerging-Adopter.png  |            |
| strategic_leader | Persona/Banner/Strategic-Leader.png  |            |
| tech_champion    | Persona/Banner/TechChampion.png      |            |
| workflow_adapter | Persona/Banner/WorkflowAdapter.png   |            |

## 2. Persona trait thumbnail  (128×128, "You also show traits of")  — 1 per persona
| Persona id       | File                               | Direct URL |
|------------------|------------------------------------|------------|
| ai_pioneer       | Persona/Hero/Ai-Pioneer.png        |            |
| domain_specialist| Persona/Hero/Domain-Specialist.png |            |
| emerging_adopter | Persona/Hero/Emerging-Adopter.png  |            |
| strategic_leader | Persona/Hero/Strategic-Leader.png  |            |
| tech_champion    | Persona/Hero/TechChampion.png      |            |
| workflow_adapter | Persona/Hero/WorkflowAdapter.png   |            |

## 3. Booth signage  (600×160, "Your Expo route")  — 1 per booth
| Booth id      | File                    | Direct URL |
|---------------|-------------------------|------------|
| agentic_coe   | Booth/Agentic CoE.png   |            |
| helix         | Booth/Helix.png         |            |
| omnicx        | Booth/OmniCX.png        |            |
| analytics_hub | Booth/Analytics Hub.png |            |
| etr           | Booth/ETR.png           |            |
