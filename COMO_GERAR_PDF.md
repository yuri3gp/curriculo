# Como Gerar o PDF do Currículo

Como não há LaTeX instalado no seu sistema, você tem algumas opções para gerar o PDF:

## Opção 1: Compilação Online (Recomendado)

### Overleaf (Gratuito)
1. Acesse [overleaf.com](https://www.overleaf.com)
2. Crie uma conta gratuita
3. Clique em "New Project" → "Upload Project"
4. Faça upload do arquivo `curriculo_yuri_teixeira.tex`
5. O PDF será gerado automaticamente

### ShareLaTeX
1. Acesse [sharelatex.com](https://www.sharelatex.com)
2. Faça upload do arquivo `.tex`
3. Compile online

## Opção 2: Instalar LaTeX Localmente

### Windows - MiKTeX
```bash
# Usando chocolatey (se instalado)
choco install miktex

# Ou baixe diretamente de: https://miktex.org/download
```

### Windows - TeX Live
```bash
# Baixe de: https://www.tug.org/texlive/windows.html
```

Após instalar, você pode compilar com:
```bash
pdflatex curriculo_yuri_teixeira.tex
```

## Opção 3: Usar Docker

Se você tem Docker instalado:

```bash
docker run --rm -v "$PWD":/data texlive/texlive pdflatex curriculo_yuri_teixeira.tex
```

## Opção 4: Extensão VS Code

Instale a extensão "LaTeX Workshop" no VS Code que pode compilar automaticamente.

---

**Recomendação:** Use o Overleaf para uma solução rápida e sem instalação!
