---
title: Tipo de recurso verifiedDomain
description: Especifica um domínio de um locatário. A propriedade **verifiedDomains** da entidade organization é uma coleção de **VerifiedDomain**.
localization_priority: Normal
author: davidmu1
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c56b7c49fc2bee4f10d338bc1bcc4cfec323ea97
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015285"
---
# <a name="verifieddomain-resource-type"></a>Tipo de recurso verifiedDomain

Namespace: microsoft.graph

Especifica um domínio de um locatário. A propriedade **verifiedDomains** da entidade [organization](organization.md) é uma coleção de **VerifiedDomain**.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|capabilities|Cadeia de caracteres|Por exemplo, "Email" ou "OfficeCommunicationsOnline".|
|isDefault|Booliano|                **true** se este é o domínio padrão associado ao locatário; caso contrário, **false**.            |
|isinitial|Booliano|**true** se esse é o domínio inicial associado ao locatário; caso contrário, **false**|
|nome|String|O nome de domínio; por exemplo, “contoso.onmicrosoft.com”.|
|tipo|String|Por exemplo, "Managed".|

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
<!-- {
  "type": "#page.annotation",
  "description": "verifiedDomain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

