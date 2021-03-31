---
title: Tipo de recurso verifiedDomain
description: Especifica um domínio de um locatário. A propriedade **verifiedDomains** da entidade organization é uma coleção de **VerifiedDomain**.
localization_priority: Normal
author: Jumaodhiss
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 8636552fa99b3389f35f22e2edccc5d13cb06482
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468979"
---
# <a name="verifieddomain-resource-type"></a>Tipo de recurso verifiedDomain

Namespace: microsoft.graph

Especifica um domínio de um locatário. A propriedade **verifiedDomains** da entidade [organization](organization.md) é uma coleção de **VerifiedDomain**.


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|capabilities|Cadeia de caracteres|Por exemplo, "Email" ou "OfficeCommunicationsOnline".|
|isDefault|Booliano|                **true** se este é o domínio padrão associado ao locatário; caso contrário, **false**.            |
|isInitial|Booliano|**true** se esse é o domínio inicial associado ao locatário; caso contrário, **false**|
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

