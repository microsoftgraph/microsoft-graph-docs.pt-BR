---
title: Tipo de recurso verifiedDomain
description: Especifica um domínio de um locatário. A propriedade **verifiedDomains** da entidade organization é uma coleção de **VerifiedDomain**.
localization_priority: Normal
ms.openlocfilehash: 088687d4450a5134c53bca6134039f7ba34a7597
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345077"
---
# <a name="verifieddomain-resource-type"></a>Tipo de recurso verifiedDomain

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Especifica um domínio de um locatário. A propriedade **verifiedDomains** da entidade [organization](organization.md) é uma coleção de **VerifiedDomain**.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|capabilities|Cadeia de caracteres|Por exemplo, "Email" ou "OfficeCommunicationsOnline".|
|isDefault|Boolean|                **true** se este é o domínio padrão associado ao locatário; caso contrário, **false**.            |
|isInitial|Booliano|**true** se esse é o domínio inicial associado ao locatário; caso contrário, **false**|
|name|String|O nome de domínio; por exemplo, “contoso.onmicrosoft.com”.|
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
