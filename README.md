# MyCod Carreira

Prévia de ferramenta pessoal para analisar perfis do LinkedIn e treinar entrevistas
para os objetivos **Full Stack Júnior** e **Telecom / O&M**.

> Status: prévia para revisão. Sem login, sem banco de dados e sem envio de dados para fora do navegador.

## Como rodar

Não há build nem dependências. Basta abrir o arquivo no navegador:

1. Clone o repositório.
2. Abra `index.html` no navegador (duplo clique ou arrastar para uma aba).

Alternativa com servidor local, se preferir:

```bash
npx serve .
```

## O que a prévia faz

- **LinkedIn:** analisa texto colado ou PDF com texto selecionável. O texto extraído aparece para revisão antes da análise.
- **Análise por regras:** verifica headline, Sobre, experiências, resultados mensuráveis, projetos, habilidades e formação. Mostra as três melhorias mais importantes, com sugestão copiável. Não usa IA.
- **Entrevista:** perguntas por objetivo e feedback sobre clareza, papel pessoal, decisão, resultado e tecnologias citadas. Também não usa IA.

## Dados de exemplo

O botão **Usar meu perfil salvo** carrega um perfil **fictício** (`Ana Exemplo Silva`). Para usar dados reais, edite o objeto `PROFILE_DEFAULT` localmente, ou preencha o formulário em "Editar meu perfil". Não versione dados reais.

## Estrutura

```
index.html          aplicação completa (HTML, CSS e JavaScript)
vendor/pdfjs/       pdf.js 3.11.174 (Apache-2.0), leitor de PDF local
```

## Privacidade

- Não coloque PDFs pessoais, planilhas com dados reais, `.env` ou chaves no repositório. O `.gitignore` já bloqueia esses tipos.
- Planilhas de atendimento usadas como referência devem ser anonimizadas e ficar fora do repositório.
