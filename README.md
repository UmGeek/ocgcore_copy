# ​ Backup da DLL – OCG API (ygopro-core Interface)

Este repositório contém um **backup de segurança** da DLL (biblioteca dinâmica) e seu cabeçalho exposto (`ocgapi.h`), ideal para mantenimento ou referência futura. A API se relaciona ao core de YGOPro (ygopro-core), a engine script de duelos de Yu-Gi-Oh! usada por diversos simuladores automatizados.

---

##  Projeto original

O repositório original do qual esse backup deriva é o **Fluorohydride/ygopro-core**, que implementa a lógica central e o processador de scripts Lua para YGOPro. Ele pode ser utilizado como biblioteca externa para servidores ou aplicativos que desejam simular duelos usando essa engine. :contentReference[oaicite:0]{index=0}

---

##  Sobre o `interface.h`

O cabeçalho define as funções exportadas pelo núcleo (`ocgapi`) para interagir com o engine interno:

- **Configuração de callbacks**:
  - `set_script_reader()`
  - `set_card_reader()`
  - `set_message_handler()`

- **Criação e controle de duelo**:
  - `create_duel()`, `create_duel_v2()`, `start_duel()`, `end_duel()`

- **Controle dos jogadores e componentes do duelo**:
  - `set_player_info()`, `process()`, `new_card()`, `query_card()`, `get_message()`, entre outras.

- Muitas dessas funções e callbacks são essenciais para integrar a engine em um sistema externo. :contentReference[oaicite:1]{index=1}

---

##  Estrutura do Repositório

