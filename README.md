# CardFlix - banners e atualizacoes

Este repositorio contem somente arquivos publicos usados pelo aplicativo.
Nunca coloque usuarios, senhas, DNS ou dados de clientes aqui.

## Banner

Coloque a imagem na pasta `banners` e adicione um item em `config.json`:

```json
{
  "id": "campanha-julho-2026",
  "active": true,
  "target": "home",
  "position": 1,
  "image": "banners/campanha-julho-2026.webp",
  "badge": "CardFlix",
  "title": "Titulo da campanha",
  "description": "Texto opcional do banner.",
  "durationMs": 15000,
  "buttonText": "",
  "actionUrl": ""
}
```

`durationMs` controla o tempo do banner. Filmes normais permanecem por 8 segundos.

## Atualizacao do APK

Envie o APK para uma Release do GitHub e atualize `appUpdate`:

```json
{
  "latestVersionCode": 7,
  "latestVersionName": "1.0.6",
  "apkUrl": "URL HTTPS DO APK",
  "mandatory": false,
  "message": "Melhorias e correcoes disponiveis."
}
```

O `latestVersionCode` precisa ser maior que o codigo instalado para o aviso aparecer.
