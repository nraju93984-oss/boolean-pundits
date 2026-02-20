🚀 BizForge: AI-Powered Branding AutomationBizForge is an end-to-end branding platform designed to transform a simple idea into a full visual and strategic identity in minutes. Built with a modern "Anti-Gravity" UI, it leverages ultra-fast inference models and a modular multi-AI workflow to democratize brand creation for startups and creators.✨ Key FeaturesAnti-Gravity UI: A weightless, modern interface featuring floating branding elements, glassmorphism, and smooth motion.High-Velocity Naming: Powered by Groq (LLaMA-3.3-70B) for near-instant brand name and tagline generation.Visual Identity Studio: Seamless integration with Stable Diffusion XL for professional logo and asset creation.Strategic Consultant: An AI Branding Assistant powered by IBM Granite for actionable business insights and strategic advice.Sentiment-Driven Tone: Real-time analysis of target market data to align brand voice and messaging.One-Click Deployment: Optimized for Vercel with a high-performance FastAPI/React monorepo structure.🛠️ Tech StackLayerTechnologyFrontendReact, Tailwind CSS, Framer MotionBackendFastAPI (Python)AI (Text)Groq LLaMA-3.3-70B, IBM Granite 4.0AI (Visual)Stable Diffusion XL (via Hugging Face API)AuthGoogle OAuth 2.0DatabaseVercel Postgres / MongoDB AtlasDeploymentVercel (Serverless Functions)📁 Project StructurePlaintextbizforge/
├── api/                # FastAPI Backend (Vercel Serverless)
│   ├── main.py         # App entry point & Routing
│   ├── auth.py         # Google Authentication logic
│   └── requirements.txt# Python dependencies
├── src/                # React Frontend
│   ├── components/     # UI Components (Floating elements)
│   ├── App.js          # Logic & Auth Provider
│   └── index.css       # Tailwind & Peach/Black theme
├── public/             # Static assets
├── vercel.json         # Deployment & Rewrite configuration
└── package.json        # Frontend dependencies
🚀 Getting Started1. PrerequisitesNode.js (v18+)Python (3.9+)API Keys: Groq API, Google Cloud Console (OAuth Client ID)2. Local SetupClone the repository:Bashgit clone https://github.com/your-username/bizforge.git
cd bizforge
Install Frontend Dependencies:Bashnpm install
Install Backend Dependencies:Bashpip install -r api/requirements.txt
Configure Environment Variables:Create a .env file in the root directory:Code snippetGROQ_API_KEY=your_groq_key
GOOGLE_CLIENT_ID=your_google_client_id
DATABASE_URL=your_postgres_url
3. ExecutionFrontend: npm start (Runs on localhost:3000)Backend: uvicorn api.main:app --reload (Runs on localhost:8000)🌐 Deployment to VercelBizForge is pre-configured for a seamless Vercel rollout:Connect your GitHub repository to the Vercel Dashboard.Vercel automatically detects the api/ folder as Serverless Functions and src/ as the frontend.Add Environment Variables in the Vercel Dashboard:GROQ_API_KEYGOOGLE_CLIENT_IDDATABASE_URLClick Deploy.🎨 Design SystemElementSpecificationHex CodePrimary BackgroundDeep Matte Black#000000Primary AccentLight Peach#FFDAB9Theme StyleAnti-GravityMinimalist / High-TechNote on Responsibility: While BizForge automates the "tedious" aspects of design, it is built to empower human creators to focus on storytelling and cultural nuance.📄 LicenseDistributed under the MIT License.
