# Claude

Repositório pessoal de configuração do Claude Code.

## O que está instalado

**ECC — Everything Claude Code** (plugin `ecc@ecc`, fonte oficial `affaan-m/ECC`)

- `.claude/settings.json` registra o marketplace do ECC e ativa o plugin.
  Toda sessão aberta com este repositório (celular, web ou PC) instala/atualiza
  o ECC automaticamente: agentes, skills, comandos e hooks.
- `.claude/rules/ecc/common/` contém as regras gerais do ECC (estilo de código,
  testes, segurança, git...). Plugins não distribuem regras, então elas ficam
  copiadas aqui.

Para adicionar regras de uma linguagem (ex.: Python, TypeScript), copie a pasta
correspondente de `rules/` do repositório do ECC para `.claude/rules/ecc/`.

## Usar no PC

```bash
git clone https://github.com/sc633/claude.git
cd claude
claude
```
