# Ocean Bird Streaming Platform

A comprehensive streaming application for Ocean Bird Foundation International educational shows including quizzes, debates, and healthcare tips.

## Features

### For Participants
- **Phone-based Recording**: Participants log in via phone to join live shows
- **Real-time Video/Audio Capture**: Stream directly from mobile devices
- **Screen Sharing**: Optional screen sharing capabilities
- **Interactive Features**: Respond to questions, participate in polls

### For Audience
- **Multi-platform Viewing**: Watch on web and mobile
- **Real-time Stream Playback**: Low-latency streaming
- **Interactive Engagement**: Live chat, polls, Q&A
- **Recording Playback**: Watch archived shows on-demand

### For Moderators
- **Stream Controls Dashboard**: Full control over live broadcasts
- **Speaker Selection**: Switch between participant feeds
- **Sound Effects**:
  - Buzz sounds for wrong answers
  - Applause for correct responses
  - Custom sound effects library
- **Background Music**: Add background music to streams
- **Audio Mixing**: Control volume levels for all participants
- **Participant Management**: Mute/unmute, remove, or spotlight participants
- **Countdown Timers**: For quiz rounds and debate segments
- **Graphics & Overlays**: Add titles, scoreboards, and branding

### Admin Backoffice
- **Show Scheduling**: Schedule upcoming educational shows
- **Video Management**: Upload and manage video clips
- **Content Library**: Organize videos by category (quizzes, debates, healthcare tips)
- **Social Media Integration**: Share clips directly to social platforms
- **Analytics Dashboard**: View viewership, engagement metrics
- **User Management**: Manage participants, moderators, and audience members
- **Settings**: Configure branding, stream quality, authentication

## Tech Stack

### Frontend
- React/Next.js - Web application
- React Native/Flutter - Mobile apps
- Socket.io - Real-time communication
- HLS/RTMP - Video streaming protocols

### Backend
- Node.js/Express - API server
- WebRTC - Peer-to-peer streaming
- FFmpeg - Video processing
- Redis - Real-time caching

### Database
- PostgreSQL - User data, shows, schedules
- MongoDB - Content metadata, analytics
- S3/Cloud Storage - Video clips storage

### Infrastructure
- Docker - Containerization
- Nginx - Reverse proxy/load balancing
- AWS/Google Cloud - Hosting & CDN

## Project Structure

```
ocean-bird-streaming-platform/
├── frontend/
│   ├── web/                 # React web app
│   ├── mobile/              # React Native mobile app
│   └── moderator-dashboard/ # Moderator control panel
├── backend/
│   ├── api/                 # Express API
│   ├── streaming/           # WebRTC/RTMP handling
│   ├── auth/                # Authentication
│   └── social-media/        # Social media integration
├── admin-backoffice/        # Admin dashboard
├── docs/                    # Documentation
└── docker-compose.yml       # Development environment
```

## Getting Started

### Prerequisites
- Node.js 16+
- PostgreSQL 12+
- Docker & Docker Compose
- FFmpeg

### Installation

```bash
# Clone repository
git clone https://github.com/oceanbirdfilms-cyber/ocean-bird-streaming-platform.git
cd ocean-bird-streaming-platform

# Install dependencies
npm install

# Setup environment variables
cp .env.example .env

# Start development environment
docker-compose up
```

## Development Roadmap

- [ ] Phase 1: Core streaming infrastructure
- [ ] Phase 2: Participant app (iOS/Android)
- [ ] Phase 3: Moderator control panel
- [ ] Phase 4: Admin backoffice
- [ ] Phase 5: Social media integration
- [ ] Phase 6: Analytics & reporting
- [ ] Phase 7: Advanced features (recording, clips, editing)

## Contributing

See CONTRIBUTING.md for guidelines.

## License

MIT License - see LICENSE file for details

## Support

For issues and feature requests, please use GitHub Issues.
