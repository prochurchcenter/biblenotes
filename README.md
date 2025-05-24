# Bible note  - bible study note Platform

Bible note is a comprehensive bible study note Platform that combines  with intuitive document management for modern bible study note professionals. Built with Next.js, TypeScript, and Tailwind CSS.

## 🚀 Features


### Bible Study Integration
- **Real-time Bible API**: Access to multiple Bible translations through the HelloAO Bible API
- **Commentary Support**: View Bible commentaries alongside translations
- **Tabbed Interface**: Multiple translations and commentaries in a single interface
- **Verse Navigation**: Easy navigation between books, chapters, and verses
- **Search & Filter**: Search within chapters and filter by verse ranges

### User Interface
- **Modern Design**: Clean, professional interface with dark mode support
- **Responsive Layout**: Works seamlessly on desktop, tablet, and mobile devices
- **Drag & Drop**: Organize notebooks with intuitive drag-and-drop functionality
- **Resizable Panels**: Customizable workspace with resizable panels
- **Real-time Collaboration**: Live updates and notifications

## 🛠️ Tech Stack

- **Frontend**:  React 18, TypeScript
- **Styling**: Tailwind CSS, shadcn/ui components
- **UI Components**: Radix UI primitives
- **Icons**: Lucide React
- **Drag & Drop**: @hello-pangea/dnd
- **Rich Text Editor**: Custom Notion-style editor
- **API Integration**: HelloAO Bible API
- **State Management**: React hooks and context

## 📦 Installation

1. **Clone the repository**
   \`\`\`bash
   git clone https://github.com/prochurchcenter/biblenotes.git
   cd biblenotes
   \`\`\`

2. **Install dependencies**
   \`\`\`bash
   npm install
   # or
   yarn install
   # or
   pnpm install
   \`\`\`

3. **Set up environment variables**
   \`\`\`bash
   cp .env.example .env.local
   \`\`\`

   Add your environment variables:
   \`\`\`env
  APP_URL=http://localhost:3000
   # Add other required environment variables
   \`\`\`

4. **Run the development server**
   \`\`\`bash
   npm run dev
   # or
   yarn dev
   # or
   pnpm dev
   \`\`\`

5. **Open your browser**
   Navigate to [http://localhost:5173/](http://localhost:5173/)

## 🏗️ Project Structure

\`\`\`
biblenote/
├── app/                          # Next.js app directory
│   ├── globals.css              # Global styles
│   ├── layout.tsx               # Root layout
│   ├── page.tsx                 # Landing page
│   ├── login/                   # Authentication pages
│   ├── register/
│   └── notebook/                # Main application
│       ├── page.tsx             # Notebooks overview
│       ├── welcome/             # Welcome page
│       ├── project/[id]/        # Individual notebook pages
│       ├── settings/            # Settings page
│       ├── trash/               # Trash management
│       └── invite/              # Team invitations
├── components/                   # React components
│   ├── ui/                      # shadcn/ui components
│   ├── bible-reader.tsx         # Bible reading interface
│   ├── commentary-reader.tsx    # Commentary interface
│   ├── notion-editor.tsx        # Rich text editor
│   ├── notion-sidebar.tsx       # Navigation sidebar
│   └── ai-chat-panel.tsx        # AI assistant
├── lib/                         # Utility libraries
│   ├── bible-api.ts            # Bible API client
│   ├── types.ts                # TypeScript definitions
│   ├── utils.ts                # Utility functions
│   └── sample-data.ts          # Sample data
├── public/                      # Static assets
└── tailwind.config.ts          # Tailwind configuration
\`\`\`

## 🔧 Configuration

### Tailwind CSS
The project uses a custom Tailwind configuration with:
- Custom color palette (primary blue, secondary yellow)
- Extended spacing and typography
- Dark mode support
- Custom animations

### shadcn/ui Components
Pre-configured components include:
- Button, Input, Textarea
- Dialog, Sheet, Popover
- Tabs, Accordion, Collapsible
- ScrollArea, Resizable panels
- And many more...

## 📚 API Integration

### Bible API
The project integrates with the HelloAO Bible API for:
- **Available Translations**: Get list of available Bible translations
- **Books & Chapters**: Navigate through Bible structure
- **Verse Content**: Display formatted Bible text with footnotes
- **Commentaries**: Access Bible commentaries and study notes

Example usage:
\`\`\`typescript
import { bibleApi } from '@/lib/bible-api'

// Get available translations
const translations = await bibleApi.getAvailableTranslations()

// Get a specific chapter
const chapter = await bibleApi.getTranslationChapter('BSB', 'GEN', 1)
\`\`\`

## 🎨 Styling Guide

### Color Palette
- **Primary**: Blue (#2563eb) - Used for main actions and highlights
- **Secondary**: Yellow (#eab308) - Used for accents and warnings
- **Gray Scale**: Custom gray palette for backgrounds and text
- **Semantic Colors**: Success (green), Error (red), Warning (yellow)

### Typography
- **Headings**: Inter font family with various weights
- **Body Text**: Optimized for readability with proper line heights
- **Code**: Monospace font for code snippets


## 📱 Responsive Design

The application is fully responsive with:
- **Mobile-first approach**: Optimized for mobile devices
- **Tablet support**: Enhanced experience on tablets
- **Desktop optimization**: Full-featured desktop interface
- **Adaptive layouts**: Components adapt to screen size

## 🚀 Deployment

### Vercel (Recommended)
1. Push your code to GitHub
2. Connect your repository to Vercel
3. Configure environment variables
4. Deploy automatically

### Other Platforms
The application can be deployed on any platform that supports Next.js:
- Netlify
- AWS Amplify
- Railway
- DigitalOcean App Platform

## 🧪 Testing

\`\`\`bash
# Run tests
npm run test

# Run tests in watch mode
npm run test:watch

# Run tests with coverage
npm run test:coverage
\`\`\`

## 📈 Performance

- **Code Splitting**: Automatic code splitting with Next.js
- **Image Optimization**: Next.js Image component for optimized images
- **Lazy Loading**: Components and routes loaded on demand
- **Caching**: Efficient caching strategies for API calls

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Development Guidelines
- Follow TypeScript best practices
- Use ESLint and Prettier for code formatting
- Write meaningful commit messages
- Add tests for new features
- Update documentation as needed

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- **shadcn/ui** - For the excellent component library
- **HelloAO Bible API** - For providing comprehensive Bible data
- **Vercel** - For hosting and deployment platform
- **Tailwind CSS** - For the utility-first CSS framework
- **React.js Team** - For the amazing React framework

## 📞 Support

For support and questions:
- Create an issue on GitHub
- Contact us at support@legalnote.com
- Visit our documentation at [docs.legalnote.com](https://docs.legalnote.com)

## 🗺️ Roadmap

### Upcoming Features
To be added SOON

### Version History


---

Built with ❤️ by the LegalNote team
