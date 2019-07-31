---
title: tipo de recurso passwordCredential
description: Contém uma credencial de senha associada a um aplicativo ou a uma entidade de serviço. A propriedade **passwordCredentials** da entidade servicePrincipalName e da entidade Application é uma coleção de **passwordCredential**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 72b07c92456ba8c1b1681b8d00b1dc5d512bc355
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009199"
---
# <a name="passwordcredential-resource-type"></a>tipo de recurso passwordCredential

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Contém uma credencial de senha associada a um aplicativo ou a uma entidade de serviço. A propriedade **passwordCredentials** da entidade [servicePrincipalName](serviceprincipal.md) e da entidade [Application](application.md) é uma coleção de **passwordCredential**.


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "secretText": "string",
  "hint": "string"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|customKeyIdentifier|Binária|            |
|endDateTime|DateTimeOffset|A data e a hora em que a senha expira. O tipo TIMESTAMP representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|keyId|Guid|            |
|startDateTime|DateTimeOffset|A data e a hora em que a senha se torna válida. O tipo TIMESTAMP representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|secretText|String| As senhas devem ter 16-64 caracteres de comprimento |
|Dica|String|  |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
