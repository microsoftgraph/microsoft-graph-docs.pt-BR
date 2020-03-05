---
title: tipo de recurso plannerAppliedCategories
description: O recurso **AppliedCategoriesCollection** representa a coleção de categorias (ou rótulos) que foram aplicados a uma tarefa. Ele faz parte do objeto plannerTask.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 61b5b8d6f883ed3e7799acd312cb71c68dd07780
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447154"
---
# <a name="plannerappliedcategories-resource-type"></a>tipo de recurso plannerAppliedCategories

Namespace: Microsoft. Graph


O recurso **AppliedCategoriesCollection** representa a coleção de categorias (ou rótulos) que foram aplicados a uma tarefa. Ele faz parte do objeto [plannerTask](plannertask.md) .
Pode haver até 6 categorias aplicadas a uma tarefa. Descrições de categoria, por `category1`exemplo `category2` , etc., fazem parte do objeto [Plan Details](plannerplandetails.md) . Este é um tipo aberto.

## <a name="properties"></a>Propriedades
As propriedades de um tipo aberto podem ser definidas pelo cliente. Nesse caso, no entanto, o cliente `category1`deve `category2`fornecer `category3`, `category4`, `category5` , e/ `category6` ou como propriedades com seus valores sendo `true` Boolean quando as categorias correspondentes são aplicadas à tarefa. O exemplo é mostrado abaixo. Quando eles não se aplicam, as propriedades são removidas automaticamente definindo seus `false` valores para o Boolean. 

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [ "String-value" ],
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
<!-- {
  "type": "#page.annotation",
  "description": "plannerAppliedCategories resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
