# Project Structure

## Overview
The Expense Tracker App is organized into a modular structure to ensure maintainability and scalability. Below is a summary of the key folders and their purposes:

### Root Directory
- **`package.json`**: Defines project dependencies and scripts.
- **`Dockerfile`**: Configuration for containerizing the application.
- **`docker-compose.yml`**: Orchestrates multi-container Docker applications.
- **`.env`**: Stores environment variables for local development.

### `src/`
Contains the main application code.
- **`app/`**: Implements the Next.js App Router structure.
  - **`dashboard/`**: Contains pages and components for the dashboard, including analytics, budgets, categories, and expenses.
  - **`sign-in/`** and **`sign-up/`**: Authentication pages.
- **`components/`**: Reusable UI components such as navigation, modals, and charts.
- **`lib/`**: Utility functions and helpers, including database and AI integrations.
- **`hooks/`**: Custom React hooks for shared logic.
- **`context/`**: Context providers for global state management.

### `docs/`
Contains documentation and diagrams.
- **`system-context.puml`**: System Context Diagram.
- **`container-diagram.puml`**: Container Diagram.
- **`sequence-add-expense.puml`**: Sequence Diagram for adding an expense.
- **`dissertation.md`**: Detailed project documentation.

### `supabase/`
Database-related files.
- **`migrations/`**: SQL scripts for database schema changes.
- **`seed.sql`**: Initial data seeding script.

### `public/`
Static assets such as images and icons.

### `scripts/`
Automation scripts for deployment and database management.

## Key Files
- **`src/lib/receipt-processor.ts`**: Handles AI-powered receipt processing.
- **`src/app/dashboard/page.tsx`**: Main dashboard page.
- **`src/components/budget/budget-overview.tsx`**: Displays budget utilization.

## Diagram Highlights
Refer to the diagrams in the `docs/` folder for a visual understanding of the system architecture and workflows.