---
layout: page
title: Rclone Desktop App
---
<script setup>
import AppHome from '@share/components/AppHome.vue'
import code from '@theme/lib/code'

const version = "1.3.0"

const downloads = [
  {
    key: 'windows',
    name: 'Windows',
    ext: '.exe',
    href: `https://release.liriliri.io/rem/REM-${version}-win-x64.exe`,
  },
  {
    key: 'mac',
    name: 'macOS Apple silicon',
    ext: '.dmg',
    href: `https://release.liriliri.io/rem/REM-${version}-mac-arm64.dmg `,
  },
  {
    key: 'mac_x64',
    name: 'macOS Intel chip ',
    ext: '.dmg',
    href: `https://release.liriliri.io/rem/REM-${version}-mac-x64.dmg`,
  },
  {
    key: 'linux',
    name: 'Linux',
    ext: '.AppImage',
    href: `https://release.liriliri.io/rem/REM-${version}-linux-x86_64.AppImage`,
  }
]

const features = [
  {
    title: 'Easy to Install',
    desc: 'Built-in Rclone, ready to use upon installation without any additional complicated operations.',
    image: '/multiwindow.png',
  },
  {
    title: 'Feature-rich',
    desc: 'Supports upload, download, copy, paste, and other operations.',
    image: '/preview.png',
  },
  {
    title: 'Easy to Use',
    desc: 'Graphical user interface, one-click operations, no need to input any commands.',
    image: '/screenshot.png',
  }
]
</script>

<AppHome 
  title="REM Rclone Desktop App" 
  subtitle="REM is a desktop application based on Rclone. It allows you to browse, organize, and transfer files across your cloud storages effortlessly."
  :code="code"
  :version="version"
  :downloads="downloads"
  :features="features"
  :changelogUrl="`https://github.com/liriliri/rem/releases/tag/v${version}`"
/>
