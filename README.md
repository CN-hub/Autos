# Autos

Sistema web de gestão para escritório de advocacia, em um único arquivo HTML (`index.html`), sem dependências a instalar.

## Recursos

- **Dashboard** com indicadores e gráficos (honorários, atendimentos, prazos, processos por área, fase e responsável, atendimentos por canal), com visão em tabela
- **Atendimentos**: fila com situação e conversão em processo
- **Processos**: número no padrão CNJ, partes, tribunal, vara, fase, andamentos
- **Prazos e agenda**: lista e calendário, com calculadora de prazo em dias úteis (feriados nacionais e recesso forense)
- **Clientes** com histórico completo
- **Financeiro**: honorários, vencimentos e baixa de pagamentos
- **Backup** automático a cada hora (mantém os 30 mais recentes), manual, download e restauração
- Login obrigatório, tema claro e escuro, menu hambúrguer, ajustes de acessibilidade (tamanho do texto, alto contraste, reduzir animações) e layout responsivo

## Como usar

Abra o `index.html` no navegador, ou publique a pasta no GitHub Pages (Settings → Pages → Deploy from a branch → `main` / root).

Os dados ficam salvos no `localStorage` do navegador. Use a aba **Backup** para baixar cópias.

## Segurança

O login (`Marcelo` / `123456@`) é uma barreira apenas visual: usuário e senha estão no código da página e qualquer pessoa com acesso ao arquivo pode lê-los. Não use este sistema para proteger dados reais de clientes em um site público. Para uso real, é necessário um servidor com autenticação de verdade.

Para trocar as credenciais, edite a linha `var CRED={u:'marcelo',p:'123456@'};` no `index.html`.
