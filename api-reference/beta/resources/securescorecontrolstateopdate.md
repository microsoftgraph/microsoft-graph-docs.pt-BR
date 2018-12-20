---
title: " tipo de recurso de secureScoreControlStateUpdate"
description: Este recurso contém o histórico de estados de controle atualizado por usuário (incluem de estados de controle padrão, Ignored, ThirdParty, revisado).
ms.openlocfilehash: ba98f2fc85f3f8e12355f9acf5d232599a7f29f7
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380963"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a>tipo de recurso de secureScoreControlStateUpdate
Contém o histórico dos Estados controle atualizados pelo usuário (incluem de estados de controle padrão, Ignored, ThirdParty, revisado).

|Propriedade	 |Tipo |Descrição |
|:--|:--|:--|
|assignedTo | string | Atribua o controle ao usuário que executará a ação |
|comment | string | Fornece um comentário opcional sobre o controle |
|estado | string | Estado do controle pode ser modificado usando-se o comando de PATCH (ex.: ignorados, thirdParty etc.) |
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
