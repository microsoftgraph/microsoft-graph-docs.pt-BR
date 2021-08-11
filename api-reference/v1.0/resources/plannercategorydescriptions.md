---
title: Tipo de recurso plannerCategoryDescriptions
description: 'O **recurso plannerCategoryDescriptions** representa os rótulos descritivos para as categorias que foram definidas para um plano. Ele pertence ao objeto de detalhes do plano. Pode haver até 6 categorias definidas. '
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 5dcb6a9b2825b2a246f1bef9b55c453c6c53c1d8c6e56a45474bfa804d8caa15
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54154914"
---
# <a name="plannercategorydescriptions-resource-type"></a>Tipo de recurso plannerCategoryDescriptions

Namespace: microsoft.graph

O **recurso plannerCategoryDescriptions** representa os rótulos descritivos para as categorias que foram definidas para um plano. Ele pertence ao [objeto de detalhes do](plannerplandetails.md) plano. Pode haver até 6 categorias definidas. 


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|category1|Cadeia de caracteres|O rótulo associado à Categoria 1|
|category2|String|O rótulo associado à Categoria 2|
|category3|String|O rótulo associado à Categoria 3|
|category4|Cadeia de caracteres|O rótulo associado à Categoria 4|
|category5|String|O rótulo associado à Categoria 5|
|category6|Cadeia de caracteres|O rótulo associado à Categoria 6|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerCategoryDescriptions"
}-->

```json
{
  "category1": "String",
  "category2": "String",
  "category3": "String",
  "category4": "String",
  "category5": "String",
  "category6": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "plannerCategoryDescriptions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

