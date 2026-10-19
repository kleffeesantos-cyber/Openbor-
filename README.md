# Openbor-

# OpenBOR para PS4 (GoldHEN)

Objetivo: gerar um `.pkg` do OpenBOR para PS4 desbloqueado.

## Plano
1. Fase 1 (este workflow): confirmar que o Actions baixa o OpenOrbis Toolchain e o codigo do OpenBOR e gerar um relatorio das dependencias.
2. Fase 2: criar `ps4/Makefile` (clang + OpenOrbis + SDL2 para PS4) e a camada de plataforma.
3. Fase 3: empacotar `eboot.bin` + `sce_sys` em `.pkg` e instalar via GoldHEN.

## Como usar a Fase 1
1. Crie um repositorio no GitHub e envie estes arquivos.
2. Aba Actions > "OpenBOR PS4 - Fase 1" > Run workflow.
3. Baixe o artefato `relatorio-fase1` e me mande o conteudo.

Os jogos (`.pak`) nao entram no pkg: depois sao copiados por FTP (porta 2121 do GoldHEN).
