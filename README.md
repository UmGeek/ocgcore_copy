# 🔹 Backup da DLL - OCG API

Este repositório contém um **backup de segurança** de uma DLL e seu respectivo cabeçalho (`ocgapi.h`), utilizados para interagir com a API OCG (provavelmente relacionada a um motor de duelos, como YGOPro/EDOPro ou derivados).

> ⚠️ **Aviso:** Este projeto não contém código-fonte completo ou implementação interna da DLL, apenas o cabeçalho público para referência.  
> O objetivo é **backup e preservação**, não distribuição comercial ou uso não autorizado.

---

## 📄 Sobre o Arquivo `interface.h`

O arquivo de cabeçalho define a interface de comunicação entre a aplicação e a DLL, incluindo:

- **Macros de exportação/importação** para compatibilidade com Windows e Linux.
- **Definições de tipos** para funções de leitura de scripts, leitura de dados de cartas e tratamento de mensagens.
- **Funções da API** para:
  - Criar e gerenciar duelos.
  - Consultar informações de cartas e do campo.
  - Enviar respostas e processar eventos.
  - Gerenciar scripts de jogo.

---

## 🔧 Funções Principais

Algumas funções expostas pela API incluem:

- `create_duel()` e `create_duel_v2()` — Inicializam um duelo.
- `start_duel()` e `end_duel()` — Controlam o ciclo de vida do duelo.
- `set_script_reader()` — Define a função de leitura de scripts.
- `query_card()` — Consulta informações detalhadas de uma carta.
- `process()` — Processa o estado atual do duelo.
- `handle_message()` — Trata mensagens enviadas pela engine.

---

## 📦 Estrutura do Repositório

