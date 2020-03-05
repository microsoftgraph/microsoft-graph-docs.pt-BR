---
title: Tipo de recurso verifiedDomain
description: Especifica um domínio de um locatário. A propriedade **verifiedDomains** da entidade organization é uma coleção de **VerifiedDomain**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 63e1f2af238aa05fbe5918ff3fc54b5a292aef21
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519481"
---
# <a name="verifieddomain-resource-type"></a>Tipo de recurso verifiedDomain

Namespace: Microsoft. Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica um domínio de um locatário. A propriedade **verifiedDomains** da entidade [organization](organization.md) é uma coleção de **VerifiedDomain**.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|capabilities|Cadeia de caracteres|Por exemplo, "Email" ou "OfficeCommunicationsOnline".|
|isDefault|Boolean|                **true** se este é o domínio padrão associado ao locatário; caso contrário, **false**.            |
|isinitial|Booliano|**true** se esse é o domínio inicial associado ao locatário; caso contrário, **false**|
|nome|String|O nome de domínio; por exemplo, “contoso.onmicrosoft.com”.|
|type|String|Por exemplo, "Managed".|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifiedDomain"
}-->

```json
{
  "capabilities": "string",
  "isDefault": true,
  "isInitial": true,
  "name": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "verifiedDomain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
