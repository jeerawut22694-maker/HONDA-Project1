## 🏭 Honda Thailand - Collaborative Dashboard

Real-time collaborative document editor with multi-user support and live updates.

### ✨ Features

- ✅ **Real-time Editing** - See changes instantly
- ✅ **Multi-user Support** - Collaborate with team members
- ✅ **Document Management** - Create, edit, delete documents
- ✅ **Auto-save** - Never lose your work (Ctrl+S)
- ✅ **Status Indicator** - See who's online
- ✅ **Responsive Design** - Works on desktop and mobile

### 🚀 Quick Start

1. **Clone and navigate to the directory:**
   ```bash
   cd collaborative-dashboard
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Setup Supabase:**
   - Create a project at [supabase.com](https://supabase.com)
   - Get your URL and ANON_KEY
   - Create these tables:
     ```sql
     -- Documents table
     CREATE TABLE documents (
       id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
       title TEXT NOT NULL,
       content TEXT DEFAULT '',
       author_id UUID NOT NULL,
       created_at TIMESTAMP DEFAULT now(),
       updated_at TIMESTAMP DEFAULT now()
     );

     -- Comments table
     CREATE TABLE comments (
       id UUID PRIMARY KEY DEFAULT gen_random_uuid(),
       document_id UUID REFERENCES documents(id) ON DELETE CASCADE,
       user_id UUID NOT NULL,
       content TEXT NOT NULL,
       created_at TIMESTAMP DEFAULT now()
     );
     ```

4. **Create `.env` file:**
   ```
   VITE_SUPABASE_URL=https://your-project.supabase.co
   VITE_SUPABASE_ANON_KEY=your-anon-key
   ```

5. **Start development server:**
   ```bash
   npm run dev
   ```

6. **Build for production:**
   ```bash
   npm run build
   ```

### 📁 Project Structure

```
collaborative-dashboard/
├── src/
│   ├── components/
│   │   ├── Dashboard.jsx      # Main dashboard
│   │   └── Editor.jsx         # Collaborative editor
│   ├── services/
│   │   └── supabase.js        # Supabase client & helpers
│   ├── store/
│   │   └── index.js           # Zustand state management
│   ├── App.jsx                # Main app component
│   ├── index.css              # Styles
│   └── main.jsx               # Entry point
├── index.html                 # HTML template
├── package.json               # Dependencies
├── vite.config.js            # Vite configuration
└── README.md                  # This file
```

### 🔒 Authentication

The app uses Supabase authentication. Users can:
- Sign up with email
- Sign in to access shared documents
- Sign out safely

### 🌐 Real-time Features

- **Live Document Updates** - Changes sync across all users
- **Presence Awareness** - See active users editing
- **Auto-save** - Save with Ctrl+S or Cmd+S
- **Document History** - Track changes over time

### 🛠 Technologies Used

- **React 18** - UI framework
- **Supabase** - Backend & Real-time DB
- **Zustand** - State management
- **Vite** - Build tool
- **CSS3** - Styling

### 📝 Environment Variables

| Variable | Description |
|----------|-------------|
| `VITE_SUPABASE_URL` | Your Supabase project URL |
| `VITE_SUPABASE_ANON_KEY` | Your Supabase anonymous key |

### 🤝 Contributing

1. Create a feature branch
2. Make your changes
3. Test thoroughly
4. Create a pull request

### 📄 License

MIT License - Feel free to use and modify!

### 📞 Support

For issues or questions, please create an issue in the repository.

---

Made with ❤️ for Honda Thailand
