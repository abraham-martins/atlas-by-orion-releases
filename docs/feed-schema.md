# ATLAS Update Feed Schema

O atualizador do ATLAS consulta `stable-feed.json` no branch `main`.

Campos usados pelo cliente:

- `schemaVersion`: versão do formato do manifesto.
- `product`: deve ser `ATLAS by Orion`.
- `channel`: `stable`.
- `version`: versão publicada, por exemplo `0.1.11.0`.
- `build`: nome legível da build.
- `publishedAt`: data/hora ISO 8601.
- `platform`: `win-x64`.
- `installerUrl`: URL direta do instalador em GitHub Releases.
- `sha256`: SHA-256 do instalador, em hexadecimal com 64 caracteres.
- `mandatory`: indica atualização obrigatória.
- `minimumSupportedVersion`: menor versão suportada.
- `releaseNotes`: lista de mudanças exibida no ATLAS.

## Regra de segurança

O ATLAS só abre o instalador quando o SHA-256 calculado localmente é idêntico ao valor publicado no manifesto. Se o hash estiver vazio, inválido ou diferente, a instalação é bloqueada.

## URL pública do feed

`https://raw.githubusercontent.com/abraham-martins/atlas-by-orion-releases/main/stable-feed.json`
