<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Moments - Web-to-Print Platform</title>
    <style>
        body { font-family: 'Segoe UI', sans-serif; line-height: 1.6; max-width: 900px; margin: 0 auto; padding: 20px; color: #333; }
        h1 { color: #2c3e50; border-bottom: 2px solid #3498db; padding-bottom: 10px; }
        h2 { color: #2980b9; margin-top: 25px; }
        .tech-stack { background: #f8f9fa; padding: 15px; border-radius: 5px; margin: 20px 0; }
        .diagram { text-align: center; margin: 30px 0; background: #f5f5f5; padding: 20px; border-radius: 5px; }
    </style>
</head>
<body>
    <h1>Moments - Collaborative Memory Book Platform</h1>
    
    <h2>About The Project</h2>
    <p>Moments is a web-to-print platform enabling collaborative creation of memory books for milestone events. Unlike traditional photobooks, our solution supports:</p>
    <ul>
        <li>Multi-contributor workflows (up to hundreds per book)</li>
        <li>Rich text-photo compositions with custom layouts</li>
        <li>End-to-end publishing workflow from collaboration to print fulfillment</li>
    </ul>
    
    <div class="diagram">
        <strong>System Architecture Diagram</strong><br>
        [Client (Next.js) → Clerk Auth → Supabase DB → Transloadit → S3 → DocRaptor → Lulu API]
    </div>
    
    <h2>Technical Implementation</h2>
    <div class="tech-stack">
        <strong>Core Stack:</strong>
        <ul>
            <li>Frontend: Next.js 14 (App Router), React 18, shadcn/ui</li>
            <li>Backend: Supabase (PostgreSQL, Edge Functions)</li>
            <li>File Processing: Transloadit pipelines with Uppy</li>
            <li>PDF Generation: DocRaptor with DearFlip.js preview</li>
        </ul>
    </div>
    
    <h3>Key Technical Challenges</h3>
    <p><strong>1. Real-time Collaboration:</strong> Implemented Supabase realtime subscriptions for page updates, requiring careful conflict resolution.</p>
    <p><strong>2. PDF Generation:</strong> DocRaptor integration needed custom CSS paged media rules to match the flipbook preview.</p>
    <p><strong>3. File Handling:</strong> Transloadit workflows with S3 storage required signed URLs and CDN optimization.</p>
    
    <h2>Project Scope</h2>
    <table border="1" cellpadding="8" cellspacing="0">
        <tr>
            <th>Component</th>
            <th>Count</th>
        </tr>
        <tr>
            <td>Responsive Pages</td>
            <td>22</td>
        </tr>
        <tr>
            <td>Interactive Modals</td>
            <td>17</td>
        </tr>
        <tr>
            <td>Core Workflows</td>
            <td>7</td>
        </tr>
    </table>
    
    <h2>Third-Party Integrations</h2>
    <ul>
        <li><strong>Clerk:</strong> Handles authentication with custom invitation flows</li>
        <li><strong>Stripe:</strong> Manages complex product variants (book sizes/paper types)</li>
        <li><strong>Lulu API:</strong> Direct print fulfillment with webhook status updates</li>
    </ul>
</body>
</html>
