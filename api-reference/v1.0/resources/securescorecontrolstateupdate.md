---
title: tipo de recurso secureScoreControlStateUpdate
description: Este recurso contém o histórico dos Estados de controle atualizados pelo usuário (os Estados de controle incluem padrão, ignorado, terceiros, revisado).
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 0fe88741da75718b1509fd4f8015a37fcf7828bf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446958"
---
#  <a name="securescorecontrolstateupdate-resource-type"></a>tipo de recurso secureScoreControlStateUpdate

Namespace: Microsoft. Graph

Contém o histórico dos Estados de controle atualizados pelo usuário (os Estados de controle incluem padrão, ignorado, terceiros, revisado).

## <a name="properties"></a>Propriedades

|Propriedade |Tipo |Descrição |
|:--|:--|:--|
|assignedTo|String|Atribui o controle ao usuário que executará a ação. |
|comment|String|Fornece comentários opcionais sobre o controle. |
|state|Cadeia de caracteres|Estado do controle, que pode ser modificado por meio de um comando PATCH (por exemplo, ignorado, terceiros). |
|updatedBy|String|ID do usuário que atualizou o estado do locatário. |
|updatedDateTime|DateTimeOffset|Hora em que o estado do controle foi atualizado. |

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
