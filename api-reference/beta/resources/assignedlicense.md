---
title: Tipo de recurso assignedLicense
description: Representa uma licença atribuída a um usuário. A propriedade **assignedLicenses** da entidade user é uma coleção de **assignedLicense**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: krbain
ms.openlocfilehash: 29dec5abd28969871376de5a55a932cea9297848
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809870"
---
# <a name="assignedlicense-resource-type"></a>Tipo de recurso assignedLicense

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma licença atribuída a um usuário. A propriedade **assignedLicenses** da entidade [user](user.md) é uma coleção de **assignedLicense**.

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|disabledPlans|Coleção de GUIDs|Uma coleção dos identificadores exclusivos de planos que foram desabilitados.|
|skuId|Guid|O identificador exclusivo da SKU.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedLicense"
}-->

```json
{
  "disabledPlans": ["guid"],
  "skuId": "guid"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "assignedLicense resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
