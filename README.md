# ATLAS by Orion — Releases

Repositório público de distribuição e atualização do **ATLAS by Orion**.

Este repositório não contém o código-fonte do produto. Ele existe para hospedar os manifestos de atualização, notas de versão e arquivos públicos de distribuição usados pelo atualizador automático do ATLAS.

## Canal Stable

Manifesto principal:

`stable-feed.json`

URL usada pelo aplicativo:

`https://raw.githubusercontent.com/abraham-martins/atlas-by-orion-releases/main/stable-feed.json`

## Versão atual

- Produto: ATLAS by Orion
- Versão: 0.1.10.9
- Build: 001A Final Update 1
- Canal: Stable
- Plataforma: Windows x64

## Segurança

Cada atualização publicada deverá informar um SHA-256. O ATLAS baixa o pacote, calcula o hash localmente e só prossegue quando o arquivo corresponder ao manifesto.

## Fluxo de publicação

1. Gerar o instalador Stable no Release Kit.
2. Publicar o instalador em uma Release do GitHub.
3. Atualizar `stable-feed.json` com versão, URL, SHA-256 e notas.
4. O ATLAS consulta o manifesto e oferece a atualização quando houver versão superior.

---

**ATLAS by Orion** — gestão e infraestrutura integrada do ecossistema Orion.
