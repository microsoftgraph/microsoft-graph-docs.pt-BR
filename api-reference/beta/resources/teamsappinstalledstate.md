---
title: Membros
description: Descreve o status atual da instalação de um teamsApp.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 82e46faccd2a91a82ba4fb7352391f58a42c33a9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517271"
---
#<a name="teamsappinstalledstate-enum-type"></a>tipo de enum teamsAppInstalledState

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve o status atual da instalação de um [teamsApp](teamsapp.md).

## <a name="members"></a>Membros

| Membro | Valor| Descrição |
|:---------------|:--------|:----------|
|notInstalled|.0|Aplicativo não está instalado para a equipe.|
|Installed|-1|App é instalado normalmente.|
|installedAndHidden|-2|App está instalado, mas oculto da exibição.|
|installedAndPermanent|-3|App permanentemente é instalado e não pode ser removido.|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsappinstalledstate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
