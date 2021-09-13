---
title: " Tipo de recurso secureScoreControlStateUpdate"
description: Esse recurso contém histórico de estados de controle atualizados pelo usuário (os estados de controle incluem Default, Ignored, ThirdParty, Reviewed).
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: ''
author: preetikr
ms.openlocfilehash: 17d35370907ac82d47b28e67b7fb4ba6c0068bb7
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59063612"
---
 #  <a name="securescorecontrolstateupdate-resource-type"></a>Tipo de recurso secureScoreControlStateUpdate
Contém o histórico dos estados de controle atualizados pelo usuário (os estados de controle incluem Default, Ignored, ThirdParty, Reviewed).

|Propriedade |Tipo |Descrição |
|:--|:--|:--|
|assignedTo | cadeia de caracteres | Atribuir o controle ao usuário que tomará a ação |
|comment | string | Fornece comentários opcionais sobre o controle |
|estado | string | O estado do controle pode ser modificado usando o comando PATCH(Ex: ignorado, thirdParty etc) |
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


