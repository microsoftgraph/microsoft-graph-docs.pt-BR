---
title: Membros
description: Descreve o status atual da instalação de um teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ca42b56e2c374dbaea1df676e3a84569b192e78c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937170"
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
