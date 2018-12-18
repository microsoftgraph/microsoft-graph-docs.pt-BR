---
title: Membros
description: Descreve o status atual da instalação de um teamsApp.
author: nkramer
ms.openlocfilehash: a73c68298c4cdf65deee68fb3bd707d50bc2475a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316790"
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
