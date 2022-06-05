---
title: " Tipo de recurso secureScoreControlStateUpdate"
description: Esse recurso contém o histórico de estados de controle atualizados pelo usuário (os estados de controle incluem Default, Ignored, ThirdParty, Reviewed).
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: security
author: preetikr
ms.openlocfilehash: 72be4693fa6b851ee587462d96451d78430a24a6
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899507"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a>Tipo de recurso secureScoreControlStateUpdate
Contém o histórico dos estados de controle atualizados pelo usuário (os estados de controle incluem Default, Ignored, ThirdParty, Reviewed).

|Propriedade |Tipo |Descrição |
|:--|:--|:--|
|assignedTo | string | Atribuir o controle ao usuário que executará a ação |
|comment | string | Fornece um comentário opcional sobre o controle |
|estado | string | O estado do controle pode ser modificado usando o comando PATCH (por exemplo: ignorado, thirdParty etc.) |
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


