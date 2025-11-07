---
layout: page
title: Rclone 桌面应用
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
    title: '开箱即用',
    desc: '内置 Rclone，下载安装即可使用。',
    image: '/multiwindow.png',
  },
  {
    title: '功能齐全',
    desc: '支持上传下载、复制粘贴等操作。',
    image: '/preview.png',
  },
  {
    title: '简单易用',
    desc: '全图形化界面，一键操作，不用输入任何命令。',
    image: '/screenshot.png',
  }
]
</script>

<AppHome 
  title="REM Rclone 桌面应用" 
  subtitle="REM 是一款基于 Rclone 的桌面应用程序，可让您轻松浏览、整理和传输各个云存储中的文件。"
  :code="code"
  :version="version"
  :downloads="downloads"
  :features="features"
  :changelogUrl="`https://github.com/liriliri/rem/releases/tag/v${version}`"
/>
