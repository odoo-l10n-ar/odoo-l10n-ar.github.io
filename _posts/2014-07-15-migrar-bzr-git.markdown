---
layout: post
title:  Cómo migrar de Launchpad a Github
date:   2014-07-July
lang:   es
author:
  name: Cristian S. Rocha 
categories: es func
section: doc
---

'''
cd [Working Directory]
bzr branch lp:~cristian-rocha/openerp-l10n-ar-localization/8.0 bzr\_l10n\_ar
git init l10n\_ar
cd l10n\_ar
bzr fast-export --plain ..\bzr\_l10n\_ar | git fast-import
git reset --hard
'''

