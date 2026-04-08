🛠 Tech Stack & System Architecture
The Engine: Distributed Monolith

Unlike a standard "everything-in-one-box" setup, this project uses a Distributed Monolith approach. While the codebase is unified for development efficiency, the services are decoupled at the infrastructure level to handle high-concurrency multi-vendor traffic.

    Framework: Yii2 (Modular Architecture) — Utilizing Gii-generated modules to isolate Vendor, Customer, and Admin logic.

    Database: MySQL (Relational Data) + Redis (Object Caching & Session Store).

    Process Management: Supervisor — Ensures 100% uptime for background workers handling heavy tasks (Email queues, PDF generation, Merchant Center syncs).

    Performance Layer: Edge CDN Caching — Aggressive caching of static assets and API responses at the network edge to minimize Time to First Byte (TTFB).

🌟 Advanced Features
Vendor Ecosystem

    KYC Onboarding Module: Secure document upload and verification flow for vendor compliance.

    Vendor Remittance Calculator: Real-time earnings breakdown including tax, commission, and currency conversion.

Logistics & Payments

    Multi-Carrier Shipping: Integrated API logic for real-time rates and tracking across multiple global carriers.

    Hybrid Payment Gateway: Support for multiple providers (Stripe, PayPal, Razorpay) with seamless failover logic.

Automation & Marketing

    Google Merchant Center: Automated XML/JSON feed generation for product synchronization.

    WhatsApp Notification Engine: Event-triggered messaging for order confirmations and shipping updates.

    Multi-Theme Support: CSS Variable-based theming allowing instant UI skinning (Dark/Light/Brand-specific).

⚙️ DevOps & Server Setup

This project is built for professional environments and requires advanced server-side configuration:

    Deployment: Optimized for 1-Hour CI/CD deployment via GitHub Actions.

    Server Requirements: * Cron Job Management: Required for scheduled inventory syncs and Google Merchant feed updates.

        Nginx Configuration: Custom caching headers and Gzip/Brotli compression settings.

        Redis: Must be enabled on the server for state-level performance.

📈 Performance Optimization

    Code Splitting: Route-based and component-based lazy loading.

    Image Optimization: Modern formats (WebP/Avif) with responsive srcset and lazy-loading.

    Asset Minification: Automated pipeline for purging unused CSS and minifying JavaScript.

🔗 Connect With Me

I am a Senior Full-Stack Developer specializing in high-performance e-commerce ecosystems and automated business logic.

    LinkedIn: (https://www.linkedin.com/in/jatinder-singh-full-stack/)
