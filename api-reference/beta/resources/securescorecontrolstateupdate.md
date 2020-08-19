---
title: " tipo de recurso secureScoreControlStateUpdate"
description: Este recurso contém o histórico de Estados de controle atualizados pelo usuário (os Estados de controle incluem Default, ignorado, terceiros).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: f3b69838a6de68938efac12acdfbcd4fd977c684
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46810402"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a>tipo de recurso secureScoreControlStateUpdate
Contém o histórico dos Estados de controle atualizados pelo usuário (os Estados de controle incluem padrão, ignorado, terceiros, revisado).

|Propriedade |Tipo |Descrição |
|:--|:--|:--|
|assignedTo | string | Atribuir o controle ao usuário que executará a ação |
|comment | string | Fornece comentários opcionais sobre o controle |
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
