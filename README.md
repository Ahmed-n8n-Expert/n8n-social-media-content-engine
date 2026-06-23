# n8n-social-media-content-engine
Automated AI Content Engine built on n8n. Generates captions, images, and videos, filters content, and schedules posts to 5 social platforms via Buffer with duplication prevention.
# 🚀 AI-Powered Social Media Content Engine (n8n + Buffer)

An enterprise-grade, fully automated AI Content Creation and Scheduling Hub built using **n8n**. This system automatically generates high-converting captions, designs visual assets (images/videos), filters the outputs, and publishes them across 5 major social media platforms simultaneously while ensuring zero post duplication.

## 🚀 Key Features

- **Automated Content Generation:** Uses advanced AI models to draft engaging captions and hashtags tailored for different audience styles.
- **Multimodal Visual Creation:** Dynamically generates custom images and short-form video assets based on trending topics or pre-defined prompts.
- **Strict Anti-Duplication System:** Integrated with a local database/datastore to log every published post. The system automatically cross-checks new content before publishing to ensure **the exact same post is never repeated**.
- **Multi-Platform Omni-Channel Publishing:** Connects seamlessly with **Buffer** to distribute content instantly to **Facebook, Instagram, LinkedIn, X (Twitter), and TikTok**.
- **Smart Content Filtering:** Features conditional logic nodes to review text structure, character limits per platform, and image resolutions before pushing to production.

## 🛠️ Built With

- **n8n** (Workflow Orchestration & Advanced Logic Routing)
- **OpenAI / DALL-E / Sora API** (For text, image, and video generation)
- **Buffer API** (For multi-network social media scheduling)
- **Supabase / Local JSON / Airtable** (For saving published logs and preventing duplication)

## 📦 How to Deploy This Workflow

1. **Import the Workflow:** Download the `workflow.json` file from this repository and upload it to your n8n canvas.
2. **Setup Database:** Create a simple table/sheet named `published_posts` with a column for `content_hash` or `caption_text` to enable the anti-duplication feature.
3. **Configure API Keys:** Add your credentials for Buffer, the AI platforms, and your database in n8n.
4. **Trigger:** Set up a Cron-Node/Schedule trigger to run this engine daily, weekly, or at specific high-traffic hours.

---
*Developed by Ahmed Tamer - AI Automation Engineer*
