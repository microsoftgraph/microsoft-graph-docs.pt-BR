---
title: " tipo de recurso de secureScoreControlStateUpdate"
description: Este recurso contém o histórico de estados de controle atualizado por usuário (incluem de estados de controle padrão, Ignored, ThirdParty, revisado).
ms.openlocfilehash: ba98f2fc85f3f8e12355f9acf5d232599a7f29f7
ms.sourcegitcommit: 8feddb85e436be5581557a199f2e46d5b4ebfa21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/22/2018
ms.locfileid: "27428837"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a>tipo de recurso de secureScoreControlStateUpdate
Contém o histórico dos Estados controle atualizados pelo usuário (incluem de estados de controle padrão, Ignored, ThirdParty, revisado).

|Propriedade |Tipo |Descrição |
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
