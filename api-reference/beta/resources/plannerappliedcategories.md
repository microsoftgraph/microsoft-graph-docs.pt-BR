---
title: tipo de recurso plannerAppliedCategories
description: O recurso **AppliedCategoriesCollection** representa a coleção de categorias (ou rótulos) que foram aplicados a uma tarefa. Ele faz parte do objeto plannerTask.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 1690eda1f8af30d388a3570d20aa28dd4cd28454
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094943"
---
# <a name="plannerappliedcategories-resource-type"></a>tipo de recurso plannerAppliedCategories

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O recurso **AppliedCategoriesCollection** representa a coleção de categorias (ou rótulos) que foram aplicados a uma tarefa. Ele faz parte do objeto [plannerTask](plannertask.md) .
Pode haver até 6 categorias aplicadas a uma tarefa. Descrições de categoria, por exemplo, `category1` `category2` etc., fazem parte do objeto [Plan Details](plannerplandetails.md) . Este é um tipo aberto.

## <a name="properties"></a>Propriedades
As propriedades de um tipo aberto podem ser definidas pelo cliente. Nesse caso, no entanto, o cliente deve fornecer,,, `category1` `category2` `category3` `category4` `category5` e/ou `category6` como propriedades com seus valores sendo `true` Boolean quando as categorias correspondentes são aplicadas à tarefa. O exemplo é mostrado abaixo. Quando eles não se aplicam, as propriedades são removidas automaticamente definindo seus valores para o `false` Boolean. 

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.plannerAppliedCategories"
}-->

```json
{
  "String-value": true
}
```

Exemplo: 

```json
{
  "category1": true,
  "category3": true,
  "category5": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "plannerAppliedCategories resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


