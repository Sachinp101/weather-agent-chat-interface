# Weather Agent Chat InterfaceThis is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://nextjs.org/docs/app/api-reference/cli/create-next-app).



A responsive chat interface that connects to a weather agent API, built with Next.js, TypeScript, and Tailwind CSS.## Getting Started



## FeaturesFirst, run the development server:



### Core Functionality ✅```bash

- Interactive chat interface with message historynpm run dev

- Real-time streaming responses from the weather agent# or

- Persistent chat history with localStorageyarn dev

- Proper error handling and loading states# or

pnpm dev

### User Interface 🎨# or

- Clean, modern design with smooth animationsbun dev

- Mobile-first responsive layout```

- Loading indicators and transitions

- Message timestampsOpen [http://localhost:3000](http://localhost:3000) with your browser to see the result.

- Distinct styling for user vs agent messages

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

### Technical Features 🔧

- Built with Next.js and TypeScriptThis project uses [`next/font`](https://nextjs.org/docs/app/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

- Tailwind CSS for styling

- Framer Motion for animations## Learn More

- Real-time streaming response display

- Keyboard shortcuts (Ctrl/Cmd + K to clear chat)To learn more about Next.js, take a look at the following resources:

- Local storage for chat persistence

- Error handling with user feedback- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.

- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

## Getting Started

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

### Prerequisites

- Node.js (v18 or later recommended)## Deploy on Vercel

- npm (comes with Node.js)

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

### Installation

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.

1. Clone the repository:
\`\`\`bash
git clone <repository-url>
cd weather-agent-chat-interface
\`\`\`

2. Install dependencies:
\`\`\`bash
npm install
\`\`\`

3. Create a \`.env.local\` file in the project root and add your college roll number:
\`\`\`
NEXT_PUBLIC_COLLEGE_ROLL_NUMBER=YOUR_ROLL_NUMBER
\`\`\`

4. Start the development server:
\`\`\`bash
npm run dev
\`\`\`

5. Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## Project Structure

\`\`\`
src/
├── app/
│   ├── globals.css          # Global styles and animations
│   └── page.tsx            # Main chat page component
├── components/
│   ├── ChatWindow.tsx      # Main chat interface container
│   ├── ChatMessage.tsx     # Individual message component
│   └── MessageInput.tsx    # Message input form component
├── hooks/
│   └── useChatState.ts     # Chat state management hook
└── services/
    └── weatherAgent.ts     # Weather agent API integration
\`\`\`

## API Integration

The chat interface connects to the weather agent API endpoint:
\`\`\`
POST https://brief-thousands-sunset-9fcb1c78-485f-4967-ac042759a8fa1462.mastra.cloud/api/agents/weatherAgent/stream
\`\`\`

### Required Headers:
\`\`\`javascript
{
  'Accept': '*/*',
  'Accept-Language': 'en-GB,en-US;q=0.9,en;q=0.8,fr;q=0.7',
  'Connection': 'keep-alive',
  'Content-Type': 'application/json',
  'x-mastra-dev-playground': 'true'
}
\`\`\`

## Available Scripts

- \`npm run dev\` - Starts the development server
- \`npm run build\` - Builds the app for production
- \`npm start\` - Runs the built app in production mode
- \`npm run lint\` - Runs the linter

## Known Limitations

- No offline support
- Limited chat history (only stored in localStorage)
- No message search functionality
- No dark mode support yet

## Future Improvements

- Add message search functionality
- Implement dark/light theme toggle
- Add message reactions or feedback
- Support for offline mode
- Add sound notifications
- Implement message delivery status indicators

## Contributing

1. Fork the repository
2. Create your feature branch: \`git checkout -b feature/YourFeature\`
3. Commit your changes: \`git commit -am 'Add some feature'\`
4. Push to the branch: \`git push origin feature/YourFeature\`
5. Submit a pull request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Screenshot
<img width="1859" height="1018" alt="Screenshot 2025-09-26 140303" src="https://github.com/user-attachments/assets/e8330cf7-0a4d-4688-a937-bf580577373e" />
