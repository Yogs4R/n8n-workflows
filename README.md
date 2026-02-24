# ⚙️ n8n Automation Workflows

![n8n](https://img.shields.io/badge/n8n-EA4B71?style=for-the-badge&logo=n8n&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)
![JSON](https://img.shields.io/badge/JSON-5E5E5E?style=for-the-badge&logo=json&logoColor=white)

Welcome to my centralized repository for **n8n** automation workflows. This project contains automated pipelines designed to fetch real-time statistics from various learning and gaming platforms, subsequently storing the data in **Supabase**. 

These workflows act as the backend data engine powering the live statistics displayed on my personal portfolio website.

## 🗂️ Workflow Directory

Below is the list of automated workflows currently maintained in this repository. All workflow files are stored in the `workflows/` directory.

| Platform | Workflow Description | Integrations | File |
| :--- | :--- | :--- | :--- |
| ![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github&logoColor=white) | Syncs GitHub profile stats (repos, stars, contributions). | n8n, Supabase | [`github.json`](./workflows/github.json) |
| ![LeetCode](https://img.shields.io/badge/LeetCode-FFA116?style=flat&logo=leetcode&logoColor=black) | Fetches LeetCode problem-solving statistics. | n8n, Supabase | [`leetcode.json`](./workflows/leetcode.json) |
| ![HackerRank](https://img.shields.io/badge/HackerRank-00EA64?style=flat&logo=hackerrank&logoColor=white) | Automates HackerRank profile data retrieval. | n8n, Supabase | [`hackerrank.json`](./workflows/hackerrank.json) |
| ![SoloLearn](https://img.shields.io/badge/SoloLearn-101728?style=flat&logo=sololearn&logoColor=white) | Updates SoloLearn coding progress and stats. | n8n, Supabase | [`sololearn.json`](./workflows/sololearn.json) |
| **Dicoding** | Syncs Dicoding academy progress and completed courses. | n8n, Supabase | [`dicoding.json`](./workflows/dicoding.json) |
| ![Roblox](https://img.shields.io/badge/Roblox-000000?style=flat&logo=roblox&logoColor=white) | Retrieves Roblox game metrics (visits, likes, favorites, members). | n8n, Supabase | [`roblox.json`](./workflows/roblox.json) |

## 🚀 How to Use

If you want to use or inspect these workflows in your own n8n instance:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Yogs4R/n8n-workflows.git
   ```
2. Open your **n8n** instance (self-hosted or cloud).
3. Create a new workflow.
4. Select Import from File in the top right menu, or simply open the `.json` file from the `workflows/` folder, copy its contents, and paste it directly into the n8n canvas.
5. Configure Credentials: Ensure you set up your own Supabase credentials and API keys for the respective platforms within n8n.

## 🛠️ Prerequisites

To run these workflows successfully, you will need:

- A running instance of [n8n](https://n8n.io).
- A [Supabase](https://supabase.com) project with the appropriate database tables configured to receive the JSON payloads.
- Necessary API keys, tokens, or scraping endpoints for GitHub, LeetCode, HackerRank, SoloLearn, Dicoding, and Roblox.

## 📄 License

This project is licensed under the MIT License.
