# Claude

Repositório pessoal de configuração do Claude Code.

## O que está instalado

**ECC — Everything Claude Code** (plugin `ecc@ecc`, fonte oficial `affaan-m/ECC`)

- **Sessões na nuvem (celular/web):** o ECC é instalado pelo *setup script* do
  ambiente "Default" (configurações do ambiente na nuvem), que roda
  `claude plugin marketplace add affaan-m/ECC` e `claude plugin install ecc@ecc`
  no início de cada sessão. O `settings.json` do repositório não basta na nuvem.
- **No PC:** `.claude/settings.json` registra o marketplace do ECC e ativa o
  plugin; o Claude Code oferece instalar ao abrir o repositório.
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
