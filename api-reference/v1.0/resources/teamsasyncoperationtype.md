---
title: tipo de enumeração teamsAsyncOperationType
description: Tipos de teamsAsyncOperation. Os membros serão adicionados aqui à medida que mais operações assíncronas forem suportadas.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 3866c41b74fc6748479099d43b268afa115dde67
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462232"
---
# <a name="teamsasyncoperationtype-enum-type"></a>tipo de enumeração teamsAsyncOperationType

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Tipos de [teamsAsyncOperation](teamsasyncoperation.md). Os membros serão adicionados aqui à medida que mais operações assíncronas forem suportadas.

## <a name="members"></a>Membros

| Membro | Valor| Descrição |
|:---------------|:--------|:----------|
|Inválido|,0|Valor inválido.|
|cloneTeam|1|Operação para clonar uma equipe.|
|archiveTeam|duas|Operação para arquivar uma equipe.|
|unarchiveTeam|3D|Operação para restaurar uma equipe arquivada.|
|createTeam|3D|Operação para criar uma equipe a partir do zero.|

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperationtype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
