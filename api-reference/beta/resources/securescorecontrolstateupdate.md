---
title: " Tipo de recurso secureScoreControlStateUpdate"
description: Esse recurso contém histórico de estados de controle atualizados pelo usuário (os estados de controle incluem Default, Ignored, ThirdParty, Reviewed).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 9e369cb863981d9998e20c17047899c8d2c02689219bdd0fef2dd56c660076d1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54176215"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a>Tipo de recurso secureScoreControlStateUpdate
Contém o histórico dos estados de controle atualizados pelo usuário (os estados de controle incluem Default, Ignored, ThirdParty, Reviewed).

|Propriedade |Tipo |Descrição |
|:--|:--|:--|
|assignedTo | cadeia de caracteres | Atribuir o controle ao usuário que tomará a ação |
|comment | string | Fornece comentários opcionais sobre o controle |
|estado | string | O estado do controle pode ser modificado usando o comando PATCH(Ex: ignorado, thirdParty etc) |
|updatedBy | cadeia de caracteres |ID do usuário que atualizou o estado do locatário |
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


