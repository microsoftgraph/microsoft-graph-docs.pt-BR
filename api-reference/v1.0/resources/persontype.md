---
title: Tipo de recurso personType
description: Representa o tipo de pessoa.
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 36310a469c5ed9289637f9701ce983db12b14fbf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36035487"
---
# <a name="persontype-resource-type"></a>Tipo de recurso personType

Representa o tipo de pessoa.


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.personType"
}-->

```json
{
  "class": "string",
  "subclass": "string"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|classe|String|O tipo de fonte de dados, como Pessoa.|
|subclasse|String|O tipo secundário de fonte de dados, como OrganizationUser.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "personType resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
