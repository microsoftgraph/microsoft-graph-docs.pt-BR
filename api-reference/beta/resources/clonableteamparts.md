---
title: tipo de enum clonableTeamParts
description: 'Descreve qual parte de uma equipe deve ser fechado. '
localization_priority: Normal
ms.openlocfilehash: 3169d6e367484248e581c12c38887e07cf5c95af
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511461"
---
# <a name="clonableteamparts-enum-type"></a>tipo de enum clonableTeamParts

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Descreve qual parte de uma [equipe](../resources/team.md) deve ser fechado. 

## <a name="members"></a>Membros

| Membro | Valor| Descrição |
|:---------------|:--------|:----------|
|Aplicativos|-1|Copie a lista de aplicativos instalados.|
|guias|-2|copia as guias no canais.|
|configurações|4*|Copia todas as definições dentro da equipe, juntamente com as configurações de chave de grupo.|
|canais|8*|Copia a estrutura de canal (mas não as mensagens no canal).|
|membros|16**|copia os membros e proprietários da equipe.|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/clonableteamparts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
