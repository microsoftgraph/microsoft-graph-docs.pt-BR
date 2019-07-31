---
title: " tipo de recurso secureScoreControlStateUpdate"
description: Este recurso contém o histórico de Estados de controle atualizados pelo usuário (os Estados de controle incluem Default, ignorado, terceiros).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 92616569a87a6ccf91c17ea7c845b8185bd33e8b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35965226"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a>tipo de recurso secureScoreControlStateUpdate
Contém o histórico dos Estados de controle atualizados pelo usuário (os Estados de controle incluem padrão, ignorado, terceiros, revisado).

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
