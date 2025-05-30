# Hugo

## Utworzenie nowego projektu z Hugo

Nowy projekt tworzymy w folderze cw4 za pomocą komend:

``` sh
hugo new site --force .
git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke.git themes/ananke
```

Następnie modyfikujemy plik `hugo.toml` i na końcu pliku dodajemy:

```
theme = 'ananke'
```

## Utworzenie nowego posta

Za pomocą hugo nowy post HTML tworzymy następująco:

``` sh
hugo new content content/posts/my-post.html
```

## Aktywowanie posta

Należy zmienić w nagłówku wygenerowanego posta zmianą draft z `true` na `false`:

```
---
title: "Web post"
date: 2025-05-29T11:33:18+02:00
draft: false
---
```

## Uruchomienie serwera hugo

W folderze z repozytorium projektu wykonujemy komendę:

``` sh
hugo serve
```

