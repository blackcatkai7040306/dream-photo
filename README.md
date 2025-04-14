<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Moments - Collaborative Memory Book Platform</title>
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
        .header {
            border-bottom: 2px solid #eee;
            padding-bottom: 20px;
            margin-bottom: 30px;
        }
        .tech-stack {
            background-color: #f8f9fa;
            padding: 15px;
            border-radius: 5px;
            margin: 20px 0;
        }
        .workflow-img {
            width: 100%;
            max-width: 800px;
            border: 1px solid #ddd;
            margin: 20px 0;
        }
    </style>
</head>
<body>
    <div class="header">
        <h1>Moments - Collaborative Memory Book Platform</h1>
        <p>A web-to-print service for creating group-contributed memory books</p>
    </div>

    <h2>About The Project</h2>
    <p>Moments is a specialized web-to-print platform designed for creating collaborative memory books. Unlike traditional photobooks created by individuals, our platform enables multiple contributors to participate in creating a rich, text-heavy memory book for special occasions.</p>
    
    <p>The workflow begins when a project organizer initiates a book project. They receive a shareable link to invite contributors who can add pages containing text, photos, or combinations. After contributions are complete, the organizer arranges the content, adds any custom pages, and submits the order. The system generates a print-ready PDF sent directly to our on-demand printing partner.</p>
    
    <p>Key differentiators from standard photobook services:</p>
    <ul>
        <li>Multi-user collaboration features</li>
        <li>Text-heavy page composition</li>
        <li>Scalable contribution system (supporting hundreds of contributors)</li>
        <li>Advanced page arrangement tools</li>
        <li>Integrated print production workflow</li>
    </ul>

    <div class="tech-stack">
        <h3>Technology Stack</h3>
        <p><strong>Frontend:</strong> React/Next.js (Vercel hosted)</p>
        <p><strong>Backend:</strong> Supabase (Database + Edge Functions)</p>
        <p><strong>Storage:</strong> S3 for PDFs and images</p>
        <p><strong>Authentication:</strong> Clerk</p>
        <p><strong>Payments:</strong> Stripe integration</p>
        <p><strong>PDF Generation:</strong> DocRaptor</p>
    </div>

    <h2>Implementation Approach</h2>
    <p>The implementation follows a component-based architecture with these key systems:</p>
    <ol>
        <li>User authentication via Clerk</li>
        <li>Page editor with Transloadit/Uppy for media handling</li>
        <li>Book customization interface with drag-and-drop functionality</li>
        <li>Order processing with Stripe integration</li>
        <li>PDF generation and print fulfillment workflow</li>
    </ol>

    <h3>Technical Challenges</h3>
    <p>Key implementation challenges include:</p>
    <ul>
        <li>Real-time collaboration features requiring careful state management</li>
        <li>Media processing pipeline with Transloadit for image transformations</li>
        <li>PDF generation with complex layout requirements</li>
        <li>Inventory synchronization with print partner API</li>
    </ul>

    <h2>Project Scope</h2>
    <p><strong>22</strong> Responsive Pages | <strong>17</strong> Modals | <strong>7</strong> Core Workflows</p>
    <p><strong>10</strong> Email Triggers | <strong>5</strong> Integrated Systems</p>

    <h2>Workflow Diagram</h2>
    <div style="text-align: center;">
        [Project Organizer] → Creates Project → [Shares Link] → [Contributors Add Content] 
        → [Organizer Arranges Book] → [PDF Generation] → [Printing Partner]
    </div>
</body>
</html>
