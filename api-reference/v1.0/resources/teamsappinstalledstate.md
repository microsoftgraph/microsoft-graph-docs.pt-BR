---
title: Membros
description: Descreve o status de instalação atual de um teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a58a0d046ef9c42f197e841ab542bf8dcb5f96f5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462246"
---
#<a name="teamsappinstalledstate-enum-type"></a>tipo de enumeração teamsAppInstalledState

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve o status de instalação atual de um [teamsApp](teamsapp.md).

## <a name="members"></a>Membros

| Membro | Valor| Descrição |
|:---------------|:--------|:----------|
|não instalado|,0|O aplicativo não está instalado na equipe.|
|instalação|1|O aplicativo está instalado normalmente.|
|installedAndHidden|duas|O aplicativo está instalado, mas oculto no modo de exibição.|
|installedAndPermanent|3D|O aplicativo está instalado permanentemente e não pode ser removido.|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsappinstalledstate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
