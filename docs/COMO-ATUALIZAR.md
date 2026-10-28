# Como manter este repositório atualizado

O WordPress da USP não se conecta ao GitHub sozinho. Por isso, sempre que mudar algo no site, registre a mudança aqui também.

## Depois de editar uma página

1. No WordPress, abra a página e vá em **Page Builder > Layouts > Importar/Exportar > Exportar**. O navegador baixa um arquivo `.json`.
2. Renomeie o arquivo com o mesmo nome do arquivo em `paginas/`, por exemplo `03-equipe.json`.
3. No GitHub, entre na pasta `paginas/`, clique em **Add file > Upload files** e envie o arquivo. Ele substitui o antigo.
4. Em **Commit changes**, descreva o que mudou (ex.: "Equipe: adiciona Umberto") e confirme.

## Depois de mudar o CSS

1. Copie todo o conteúdo do **Custom CSS** do site.
2. No GitHub, abra `css/labmaker.css`, clique no **lápis (Edit)**, apague tudo, cole o novo e faça o **Commit changes** com uma descrição.

## Voltar uma versão antiga

Abra o arquivo no GitHub e clique em **History**. Escolha a versão desejada, clique em **View file** e depois em **Raw** (ou **Download**). Use esse arquivo para restaurar a página ou o CSS no WordPress.

## Cuidados

- O repositório deve ser **privado**: os layouts contêm nomes e telefone de contato da equipe.
- **Nunca** envie senhas, senhas de aplicativo ou dados de login para o repositório.
