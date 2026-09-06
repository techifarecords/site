# IFÁ Records — site

Site institucional de página única. Tudo vive em **um único arquivo**: `index.html`.
Fontes, logo, grafismo e favicon estão embutidos — a página não depende de nenhum
arquivo externo, só do Google Fonts para a Archivo.

## Ver localmente

Dois cliques em `index.html`. Abre no navegador como qualquer site.

## Publicar

O repositório já está pronto para **GitHub Pages**: em _Settings → Pages_, aponte
para a branch `main` e a pasta raiz (`/`). O `index.html` na raiz é servido direto.

Para usar o domínio próprio, crie um arquivo `CNAME` na raiz contendo apenas:

```
ifarecords.com.br
```

…e aponte o DNS do domínio para o GitHub Pages.

## Regerar a página

A pasta `_fonte/` guarda o que gera o `index.html`: o script `build_site.py`, os SVGs
do logo e do grafismo, e os arquivos da fonte Monument. Você não precisa dela para
publicar — só para editar o site.

```bash
cd _fonte
python build_site.py ../index.html
```

## Pendências

- **Redes sociais.** O Instagram aponta para `instagram.com/ifa.records`. TikTok e
  YouTube ainda estão com links genéricos, propositalmente — trocar antes de divulgar.
- **Imagem de compartilhamento.** Falta a imagem que aparece ao colar o link no
  WhatsApp/Instagram. Só dá para gerar depois que o domínio estiver no ar.

## Licença das fontes

**PP Monument Extended** veio no pacote da marca com licença *Free for Personal Use*.
Está embutida aqui num subconjunto mínimo (só os caracteres usados, ~10 KB). Para uso
comercial em produção, a IFÁ precisa comprar a licença na
[Pangram Pangram](https://pangrampangram.com/products/monument-extended).

**Archivo** é do Google Fonts (SIL Open Font License) — livre para uso comercial.

## Diretrizes

Segue o *Manual de Identidade Visual — Ifá Records*:

- Cores prioritárias: `#231104` · `#4F2709` · `#BC6320` · `#FF8B00` · `#F9F7E1`
- Logo prioritário (símbolo > tipografia > complemento) no topo
- Monument Extended nos títulos, Archivo medium/semibold nos subtítulos, Archivo regular no corpo
- Grafismo: as linhas internas do símbolo, vetor extraído do próprio manual
