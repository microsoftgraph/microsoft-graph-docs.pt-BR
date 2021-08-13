---
title: Tipo de recurso secureScoreControlStateUpdate
description: Esse recurso contém o histórico dos estados de controle atualizados pelo usuário (os estados de controle incluem Default, Ignored, ThirdParty, Reviewed).
localization_priority: Normal
author: preetikr
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3268b5f537b8538173031b3367ff0e13d2873a906dfe01a5b6d6562070812d56
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54146360"
---
#  <a name="securescorecontrolstateupdate-resource-type"></a>Tipo de recurso secureScoreControlStateUpdate

Namespace: microsoft.graph

Contém o histórico dos estados de controle atualizados pelo usuário (os estados de controle incluem Default, Ignored, ThirdParty, Reviewed).

## <a name="properties"></a>Propriedades

|Propriedade |Tipo |Descrição |
|:--|:--|:--|
|assignedTo|Cadeia de caracteres|Atribui o controle ao usuário que tomará a ação. |
|comment|String|Fornece comentários opcionais sobre o controle. |
|state|Cadeia de caracteres|Estado do controle, que pode ser modificado por meio de um comando PATCH (por exemplo, ignorado, thirdParty). |
|updatedBy|Cadeia de caracteres|ID do usuário que atualizou o estado do locatário. |
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

