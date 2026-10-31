+++
title = "Coverage-Guided Fuzzer"
description = "Cattura i bug edge-case con la generazione intelligente di input"
weight = 6
date = 2024-05-01

[extra]
github = "https://github.com/example/coverage-fuzzer"
card_links = [
  { url = "https://example-coverage-fuzzer.rtfd.io", text = "Docs", icon = "globe" },
  { url = "https://discord.gg/covfuzz", text = "Discord", icon = "discord" },
]
tags = ["rust", "llvm", "fuzzing"]
+++

Un motore di fuzzing guidato dalla copertura che strumenta i binari compilati per massimizzare l'esplorazione del percorso del codice. Si integra con i sistemi di compilazione esistenti, correla i crash con input di riproduzione minimi e fornisce una dashboard di triage per deduplicare e stabilire le priorità dei risultati. Progettato per il fuzzing continuo su larga scala con supporto di prima classe per il feedback del disinfettante e grammatiche di input di test strutturate.
