---
title: " tipo de recurso de secureScoreControlStateUpdate"
description: Este recurso contém o histórico de estados de controle atualizado por usuário (incluem de estados de controle padrão, Ignored, ThirdParty, revisado).
localization_priority: Normal
ms.openlocfilehash: 8d8c3122a6263ebc7b10b5edfb823953e2d587fc
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641726"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a>tipo de recurso de secureScoreControlStateUpdate
Contém o histórico dos Estados controle atualizados pelo usuário (incluem de estados de controle padrão, Ignored, ThirdParty, revisado).

|Propriedade |Tipo |Descrição |
|:--|:--|:--|
|assignedTo | string | Atribua o controle ao usuário que executará a ação |
|comment | string | Fornece um comentário opcional sobre o controle |
|state | string | Estado do controle pode ser modificado usando-se o comando de PATCH (ex.: ignorados, thirdParty etc.) |
|updatedBy | string |ID do usuário que atualizou o estado de locatário |
|updatedDateTime | DateTimeOffset? |Tempo no qual controle estado foi atualizado |
 ## <a name="json-representation"></a>Representação JSON
 Veja a seguir uma representação JSON do recurso.
 <!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.secureScoreControlStateUpdate"
}-->
 ```json
{
  "assignedTo": "String",
  "comment": "Double",
  "state": "Double",
  "updatedBy": "Double",
  "updatedDateTime": "Double"
}
 ```
 <!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlStateUpdate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
