# LabMaker EESC-USP: site

Código e layouts do site do **LabMaker**, o laboratório de impressão 3D da Escola de Engenharia de São Carlos (EESC-USP).
Site no ar: https://sites.usp.br/labmaker

O site roda em WordPress (rede sites.usp.br), com o tema da USP, o **SiteOrigin Page Builder** e o plugin **SiteOrigin CSS**. Este repositório guarda tudo o que foi personalizado, para servir de **backup**, **histórico de versões** e **documentação**.

## Estrutura

```
css/
  labmaker.css       → todo o CSS do site (Aparência > Custom CSS)
paginas/
  01-inicio.json … 14-creditos.json
                     → layout de cada página no Page Builder
imagens/
  logos brancas do rodapé, imagem padrão de notícia e foto padrão da equipe
docs/
  COMO-ATUALIZAR.md  → como restaurar e como registrar mudanças
```

## O que o site tem

- Páginas montadas em blocos (Page Builder), com largura total e visual no padrão EESC (azul #224a85)
- Rodapé próprio em todas as páginas, com as logos da EESC, da Biblioteca e do CETEPE
- Animações de entrada em cascata ligadas à rolagem, com respeito à opção "reduzir movimento"
- Modo escuro automático, que segue a configuração do sistema do visitante
- Notícias automáticas (RSS) de portais de tecnologia e de portais internacionais de impressão 3D, com filtros de conteúdo
- Museu de Projetos, Galeria, Equipe, Guia de materiais, Perguntas frequentes e páginas das impressoras

## Restaurar uma página

1. No WordPress, abra a página e vá na aba **Page Builder**.
2. Clique em **Layouts > Importar/Exportar** e envie o JSON correspondente da pasta `paginas/`.
3. Escolha **Substituir conteúdo atual**, clique em **Atualizar** e depois em **Delete Cache**.

## Restaurar o CSS

**Aparência > Custom CSS** → apague tudo → cole o conteúdo de `css/labmaker.css` → salvar → **Delete Cache**.

> Regra de ouro do CSS: trechos novos sempre **antes** da seção `8. ACESSIBILIDADE`, que deve ser o último bloco do arquivo.

## Imagens

As logos e imagens padrão devem estar na Mídia do site com **os mesmos nomes de arquivo**, porque o rodapé e algumas páginas encontram as imagens pelo nome.
