---
layout: post
title: ubuntu 11.04 dil sorunu
---
Ubuntu 11.04' ü yeni yükleyince **Language Support** ekranı gelmediğinden dil
ayarlarınızı yapamıyorsanız sorunu aşağıdaki şekilde çözebilirsiniz;

`Uygulamalar –> Ana menü` seçelim ve soldaki sekmeden `Sistem` altındaki
`Yönetim` menüsüne tıklayalım. Sağdaki `Dil Desteği -> Özellikler` 'e
tıklayalım, sonrasında **commant** bölümüne şu yazıyı yazalım ve kaydedelim;

	env LANG=”en_US.UTF8” /usr/bin/gnome-language-selector

Artık `Uygulamalar –> Ana menü` ile açabilirsiniz.


