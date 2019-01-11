---
title: Membros
description: Descreve o status atual da instalação de um teamsApp.
author: nkramer
localization_priority: Normal
ms.openlocfilehash: 4e453a28b0c3ebc2957cf7e1a92a846e8e4758e6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27847569"
---
#<a name="teamsappinstalledstate-enum-type"></a>tipo de enum teamsAppInstalledState

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Descreve o status atual da instalação de um [teamsApp](teamsapp.md).

## <a name="members"></a>Membros

| Membro | Valor| Descrição |
|:---------------|:--------|:----------|
|notInstalled|0|Aplicativo não está instalado para a equipe.|
|instalado|1|App é instalado normalmente.|
|installedAndHidden|2|App está instalado, mas oculto da exibição.|
|installedAndPermanent|3|App permanentemente é instalado e não pode ser removido.|
