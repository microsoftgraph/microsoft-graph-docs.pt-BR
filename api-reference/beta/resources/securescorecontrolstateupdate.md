---
title: " tipo de recurso secureScoreControlStateUpdate"
description: Este recurso contém o histórico de Estados de controle atualizados pelo usuário (os Estados de controle incluem Default, ignorado, terceiros).
localization_priority: Normal
ms.openlocfilehash: 24febeb4bfb055e89e59cdb4f79c8b60c6c40347
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343357"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a>tipo de recurso secureScoreControlStateUpdate
Contém o histórico dos Estados de controle atualizados pelo usuário (os Estados de controle incluem padrão, ignorado, terceiros, reVisado).

|Propriedade |Tipo |Descrição |
|:--|:--|:--|
|assignedTo | string | Atribuir o controle ao usuário que executará a ação |
|comentário | string | Fornece comentários opcionais sobre o controle |
|estado | string | O estado do controle pode ser modificado usando o comando PATCH (ex: ignorado, terceiros etc.) |
|updatedBy | string |ID do usuário que atualizou o estado do locatário |
|updatedDateTime | DateTimeOffset |Hora em que o estado de controle foi atualizado |
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
  "comment": "string",
  "state": "string",
  "updatedBy": "string",
  "updatedDateTime": "DateTimeOffset"
}
 ```
 <!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlStateUpdate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
