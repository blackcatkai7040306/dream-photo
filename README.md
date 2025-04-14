<!DOCTYPE html>
<html lang="en">
<head>
    <style>
        body {
            font-family: 'Segoe UI', Arial, sans-serif;
            line-height: 1.6;
            color: #333;
            max-width: 900px;
            margin: 0 auto;
            padding: 20px;
        }
        h1, h2 {
            color: #2c3e50;
        }
        .diagram {
            background-color: #f8f9fa;
            padding: 15px;
            border-radius: 5px;
            margin: 20px 0;
            text-align: center;
        }
        .tech-stack {
            display: flex;
            flex-wrap: wrap;
            gap: 10px;
            margin: 15px 0;
        }
        .tech-item {
            background-color: #e1f5fe;
            padding: 5px 10px;
            border-radius: 3px;
            font-size: 0.9em;
        }
    </style>
</head>
<body>

<h1>AI-Assisted Development Support Specialist</h1>

<h2>About the Project</h2>
<p>This role supports multiple web application projects built with modern technologies and AI-assisted development tools. The primary focus is troubleshooting, optimization, and guidance rather than full-scale development.</p>

<p>The projects involve:</p>
<ul>
    <li>React-based frontends with TypeScript and TailwindCSS</li>
    <li>Supabase backend services (database, auth, storage)</li>
    <li>Vercel-hosted deployments</li>
    <li>AI-assisted development workflow using Windsurf or similar tools</li>
</ul>

<div class="diagram">
    <h3>Project Architecture Flow</h3>
    <p>[React Frontend] ↔ [Supabase API Layer] ↔ [PostgreSQL Database]</p>
    <p>↑<br>Vercel Deployment</p>
</div>

<h2>Technical Challenges and Solutions</h2>
<h3>Common Issues Faced:</h3>
<ol>
    <li><strong>AI-Generated Code Limitations</strong>:
        <p>Windsurf/Copilot sometimes produces non-optimal or outdated patterns. Requires validation of:</p>
        <ul>
            <li>Proper TypeScript typing</li>
            <li>Correct Supabase query patterns</li>
            <li>React hooks best practices</li>
        </ul>
    </li>
    
    <li><strong>Supabase-Vercel Integration</strong>:
        <p>Environment variable management and proper CORS configuration often need adjustment during deployment.</p>
    </li>
    
    <li><strong>TypeScript Type Definitions</strong>:
        <p>AI tools frequently miss proper type generation for Supabase responses, requiring manual intervention.</p>
    </li>
</ol>

<h2>Technical Stack</h2>
<div class="tech-stack">
    <span class="tech-item">React 18+</span>
    <span class="tech-item">TypeScript 5+</span>
    <span class="tech-item">TailwindCSS 3+</span>
    <span class="tech-item">Supabase</span>
    <span class="tech-item">PostgreSQL</span>
    <span class="tech-item">Vercel</span>
    <span class="tech-item">Windsurf/Copilot</span>
</div>

<h2>Working Methodology</h2>
<p>The support process involves:</p>
<ol>
    <li>Issue triage via chat/screenshare</li>
    <li>Analysis of AI-generated code segments</li>
    <li>Recommendations for optimization</li>
    <li>Debugging assistance</li>
    <li>Deployment troubleshooting</li>
</ol>

<p>Typical workflow focuses on incremental improvements rather than complete rewrites, maintaining the AI-assisted development approach while ensuring production-quality output.</p>

</body>
</html>
