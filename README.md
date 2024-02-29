# VerifiedCrowdFunder: A World ID-Enabled Crowdfunding Platforme

Welcome to VerifiedCrowdFunder, the innovative crowdfunding platform that integrates Worldcoin's World ID for real human verification. By leveraging Next.js, TailwindCSS, and the World ID SDK, we ensure every creator and supporter on our platform is a verified human. This approach significantly reduces fraud risks and ensures equitable opportunities for funding various projects, from tech innovations to social causes.

## Getting Started with VerifiedCrowdFunder

Ensure you're using the correct Node.js version and set up your development environment.

```bash
nvm use 18
pnpm i && pnpm dev
```

## Environment Configuration
Copy .env.example to .env.local.
Replace the placeholder values with your specific configurations:

```env
FAPP_ID=CrowdVerify_2024
ACTION_ID=EquitableFunding
```
These values are crucial for integrating the World ID SDK into our platform, enabling us to verify the identity of each user uniquely and securely.

## Launching the Platform
Open http://localhost:3000 to see your platform live. The development server allows you to test the full functionality in real-time.

## API Integration
This template includes an API route (/api/verify) for verifying the proof returned by the World ID widget. Customize src/pages/api/verify.ts for any backend functions your platform requires.

## Frontend Customization
Start customizing the platform by editing src/pages/index.tsx. Implement the onSuccess function to define how your platform reacts once a user's proof has been verified.

## Learn More
To dive deeper into the technologies powering VerifiedCrowdFunder, explore the following resources:

Next.js Documentation - Discover more about Next.js features and API.
World ID Documentation - Understand how World ID works and how it can be integrated into your projects.

## Deploying Your Platform
Deploying your Next.js app is straightforward with the Vercel Platform, created by the makers of Next.js. Check the Next.js deployment documentation for detailed instructions.

Join us in revolutionizing crowdfunding with verified human participation. Together, we can create a more equitable and fraud-free funding environment.






This is a template repository for creating a new project using Next.js, TailwindCSS, and the [World ID SDK](https://id.worldcoin.org). This template isn't intended for use cases that require on-chain verification, but rather for use cases that leverage off-chain web backend verification.

## Getting Started

First, set the correct Node.js version using `nvm` and run the development server:

```bash
nvm use 18
pnpm i && pnpm dev
```

Copy `.env.example` to `.env.local` and add your World ID App ID and Action Name to the appropriate variables.

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

This template includes an API route to verify the proof returned by the IDKit widget at `/api/verify`. Edit `src/pages/api/verify.ts` to handle any backend functions you need to perform.

You can start editing the page by modifying `src/pages/index.tsx`. The page auto-updates as you edit the file. Edit the `onSuccess` function to define frontend behavior once the proof has been verified.

The `src/pages/api` directory is mapped to `/api/*`. Files in this directory are treated as [API routes](https://nextjs.org/docs/api-routes/introduction) instead of React pages.

## Learn More

To learn more about Next.js and World ID, take a look at the following resources:

-   [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
-   [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.
-   [World ID Documentation](https://docs.worldcoin.org/) - learn about World ID features and API.

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out the [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.
