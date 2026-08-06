---
description: Duplica o template brand-motion-template para iniciar um projeto novo, sem alterar o template original
argument-hint: nome-do-cliente
---

Duplique o repositório template `arcocontents-dotcom/brand-motion-template` para criar um projeto novo chamado `$ARGUMENTS`, como pasta irmã do template (nunca dentro dele).

Rode, em sequência, usando caminhos absolutos (não cd relativo):

1. cd "/Volumes/PortableSSD/Gestão/Claude IA" && gh repo create $ARGUMENTS --template arcocontents-dotcom/brand-motion-template --public --clone
2. cd "/Volumes/PortableSSD/Gestão/Claude IA/$ARGUMENTS" && npm install

Confirme ao final que a pasta nova ficou em /Volumes/PortableSSD/Gestão/Claude IA/$ARGUMENTS — como irmã de brand-motion-template, brs e bidoia, nunca como subpasta de nenhuma delas.

Não modifique o repositório arcocontents-dotcom/brand-motion-template em nenhuma hipótese — ele é somente a base, nunca o destino de alterações.

Depois rode:
git add .claude/commands/novo-projeto.md && git commit -m "fix: garante caminho absoluto correto para Claude IA no /novo-projeto" && git push
