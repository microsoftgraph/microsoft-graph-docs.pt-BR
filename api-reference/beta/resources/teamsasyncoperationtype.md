---
title: tipo de enum teamsAsyncOperationType
description: Tipos de teamsAsyncOperation. Os membros serão adicionados aqui assíncrono conforme mais operações são suportadas.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4de95db194bf41939521b53f06614b46b6afae99
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29516564"
---
# <a name="teamsasyncoperationtype-enum-type"></a>tipo de enum teamsAsyncOperationType

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Tipos de [teamsAsyncOperation](teamsasyncoperation.md). Os membros serão adicionados aqui assíncrono conforme mais operações são suportadas.

## <a name="members"></a>Membros

| Membro | Valor| Descrição |
|:---------------|:--------|:----------|
|Invalid|.0|Valor inválido|
|cloneTeam|-1|Operação para clonar uma equipe.|
|archiveTeam|-2|Operação de uma equipe de arquivamento.|
|unarchiveTeam|-3|Operação de restauração uma equipe arquivada.|
|createTeam|-3|Operação para criar uma equipe a partir do zero.|

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperationtype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
