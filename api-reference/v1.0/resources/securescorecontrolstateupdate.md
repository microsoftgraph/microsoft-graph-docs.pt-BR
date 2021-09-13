---
title: Tipo de recurso secureScoreControlStateUpdate
description: Esse recurso contém o histórico dos estados de controle atualizados pelo usuário (os estados de controle incluem Default, Ignored, ThirdParty, Reviewed).
ms.localizationpriority: medium
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 1e896d1b63a9b6024b62e5d7ada95049e2f717f1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59084087"
---
#  <a name="securescorecontrolstateupdate-resource-type"></a>Tipo de recurso secureScoreControlStateUpdate

Namespace: microsoft.graph

Contém o histórico dos estados de controle atualizados pelo usuário (os estados de controle incluem Default, Ignored, ThirdParty, Reviewed).

## <a name="properties"></a>Propriedades

|Propriedade |Tipo |Descrição |
|:--|:--|:--|
|assignedTo|String|Atribui o controle ao usuário que tomará a ação. |
|comment|String|Fornece comentários opcionais sobre o controle. |
|state|Cadeia de caracteres|Estado do controle, que pode ser modificado por meio de um comando PATCH (por exemplo, ignorado, thirdParty). |
|updatedBy|String|ID do usuário que atualizou o estado do locatário. |
|updatedDateTime|DateTimeOffset|Hora em que o estado de controle foi atualizado. |

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
  "comment": "String",
  "state": "String",
  "updatedBy": "String",
  "updatedDateTime": "String (timestamp)"
}
 ```
 <!-- {
  "type": "#page.annotation",
  "description": "secureScoreControlStateUpdate resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

