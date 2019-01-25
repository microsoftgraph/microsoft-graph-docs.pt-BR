---
title: tipo de enum teamsAsyncOperationStatus
description: Descreve o status atual de um teamsAsyncOperation.
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: e9138adcc646677955a12091a3fb15badfd39f13
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511706"
---
# <a name="teamsasyncoperationstatus-enum-type"></a>tipo de enum teamsAsyncOperationStatus

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve o status atual de um [teamsAsyncOperation](teamsasyncoperation.md).

## <a name="members"></a>Membros

| Membro | Valor| Descrição |
|:---------------|:--------|:----------|
|Invalid|.0|Valor inválido|
|notStarted|-1|A operação não foi iniciada.|
|InProgress|-2|A operação está sendo executado.|
|Succeeded|-3|A operação foi bem-sucedida.|
|com falha.|4*|Falha na operação.|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsasyncoperationstatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
