# CellGestor — Management Platform for Phone Repair Shops

> Public summary. The source code is private; this repository describes what was built, how, and with which stack.

CellGestor centralizes the operation of mobile phone repair shops, from the first quote to the warranty. Service orders, customers, devices, parts inventory, counter sales, reports and WhatsApp communication live in one place, replacing scattered spreadsheets and tools.

**My role:** Full-stack development of the API, the web app and the product's subscription model.

## Key features

- **Service orders** — full history, photos and media, parts, quotes, receipts and PDF generation.
- **Customers and devices** — registration with IMEI lookup and the complete history of each device.
- **Inventory and sales** — parts stock, counter sales, warranties and returns.
- **Reports and analytics** — financial reports and team indicators.
- **WhatsApp and notifications** — operational messages to customers, real-time updates and email.
- **Multi-company SaaS** — authentication, profiles, permissions and several companies per account.
- **Subscriptions** — Stripe billing for monthly and yearly plans.
- **Responsive web app** for desktop, tablet and phone, with LGPD-aware handling of personal data.

## Tech stack

| Layer | Technologies |
|---|---|
| Backend | NestJS, TypeScript, Prisma, Passport JWT, Socket.IO, @nestjs/schedule, throttling, PDFKit, Nodemailer |
| Data | PostgreSQL, Redis, AWS S3 |
| Frontend | Next.js, React, TypeScript, Tailwind CSS, shadcn/ui + Radix UI, React Hook Form |
| Payments | Stripe |
| Quality & infra | Jest, Supertest, Vitest, Docker, Swagger / Scalar |
