# DBU — Database Utility

Utilitário TUI clássico para navegação e edição de bancos de dados no formato DBF, recompilado para Harbour.

> Preservação do DBU original do CA-Clipper (Computer Associates, 1990–1993), recompilado com o compilador Harbour para manter compatibilidade em sistemas modernos.

## Funcionalidades

- Navegação e edição interativa de arquivos `.dbf`
- Suporte a até 6 arquivos abertos simultaneamente com índices e relações
- Filtros por expressão e relações entre tabelas
- Salvar e restaurar configurações de visualização em arquivos `.vue`
- Modos cor e monocromático
- Abertura exclusiva (`/E`) para ambientes não compartilhados

## Stack

| Componente | Tecnologia |
|---|---|
| Linguagem | Harbour (CA-Clipper) |
| Build | hbmk2 / rmake |
| Interface | TUI (terminal de texto) |
| Banco de dados | DBF / NTX |

## Uso

```bash
dbu                          # abre sem arquivo
dbu banco.dbf                # abre arquivo diretamente
dbu arquivo.vue              # abre com view salva
dbu banco.dbf /M             # modo monocromático
dbu banco.dbf /E             # modo exclusivo (não compartilhado)
```

## Build

```bash
hbmk2 dbu.hbp
```

Ou usando o makefile original:
```bash
rmake dbu
```

## Origem

Copyright (c) 1990–1993, Computer Associates International Inc.  
Recompilado e preservado para Harbour por [jairslima](https://github.com/jairslima).

## Autor do fork

**Jair Lima** — [github.com/jairslima](https://github.com/jairslima)