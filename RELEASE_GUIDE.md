# Guia de Release (GitHub Releases)

Publicar o executável em **Releases** é a forma mais profissional.

## Passo a passo

1. **Build** no Unity
   - `File > Build Settings > Build` (Windows/Mac/Linux)
   - Gere uma pasta `Build/` com os binários.

2. **Compacte**
   - Crie um arquivo `.zip` com a pasta de build (ex.: `tictactoe-3d-win64.zip`).

3. **Crie uma Release no GitHub**
   - Vá em **Releases** → **Draft a new release**
   - **Tag**: `v0.1.0` (ou semelhante)
   - **Title**: `v0.1.0 - Primeira Release`
   - **Descrição**: o que mudou (changelog resumido)
   - **Anexe** o `.zip` do executável

4. **Publique** a Release.

5. **Linke no README**
   - Adicione um link direto na seção *Como Rodar*:
     ```md
     ➜ Baixe o executável em **Releases**: https://github.com/ValencoSilva/tictactoe-3d-gpt4/releases
     ```

## Dicas
- Não faça commit de executáveis pesados no `main`.
- Use **tags semânticas** (vMAJOR.MINOR.PATCH).
- Para builds automáticos, configure **GitHub Actions** futuramente.
