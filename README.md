#  Reverie

Share your private moments, securely.

## Overview and Motivation

Reverie is an open-source, self-hosted journaling and content-sharing platform designed for individuals who want to share private moments with family and friends, while maintaining full ownership and control over their data. Unlike social media platforms that monetize user data and lack strong privacy, Reverie enables secure and controlled sharing with only the people you choose.

I was motivated to build Reverie for two main reasons: First, existing platforms like Day One fall short in terms of privacy, control, and workflow integration. Second, I was eager to build a new Ruby on Rails application and explore modern Rails features. Ultimately, I want a platform that puts privacy and control first, while also being a fun and educational project for me to build.

Self-hosting requires some commitment, including finding a hosting solution (such as a Virtual Private Server) and managing backups, users, and general application/server maintenance. However, this is the price for true data ownership and peace of mind.

_Sounds like: "reh·vuh·ree"_

> Reverie: A state of being pleasantly lost in one's thoughts; a daydream. This project aims to create a space for those personal reflections, shared intimately with loved ones.

## Planned Features

Reverie is currently in the early stages of development. Here's a list of the core features I plan to implement, focusing on privacy, control, and ease of use:

**Core Features**
- **Private Posts:** Ability to create and share posts with a select group of family and friends.
- **End-to-End Encryption:** Ensuring that only you and your intended recipients can access your content. _(Implement using client-side encryption with libsodium or Web Crypto API)_
- **Granular Access Control:** Ability to specify exactly who can see each post (individuals, groups, tag-based access). _(Implement with per-post encryption keys and recipient-based key sharing)_
- **Markdown Support:** Ability to write posts in Markdown for easy import from Obsidian. _(Use Kramdown with. custom converter for Obsidian Flavoured Markdown)_
- **Social Login:** Easy access for family members using existing social media accounts (Google, Meta, etc.).  _(Implement using OmniAuth)_
- **Media Attachments:** Ability to securely attach photos and videos to posts. _(Encrypt files before upload using AES-GCM and store in S3-compatible storage)_
- **Comments and Reactions:** Allowing for interaction and engagement with your shared content. _(Encrypt comments and reactions in the same way as posts)_

**Future Enhancements / Experiments:**
- API access for adding/updating posts.
- Mobile app support.
- AI-powered post summarization and tagging.
- "Bring Your Own Key" (BYOK) encryption. _(Allow users to encrypt their data with a key they fully control)_

## Getting Started

### Prerequisites

- A Linux-based VPS (DigitalOcean, Linode, Hetzner, etc.)
- Experience with Ruby on Rails 8 and PostgreSQL

### Installation

## Contributing

If you have ideas, improvements, or bug fixes, feel free to open an issue or submit a pull request.
