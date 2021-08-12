---
title: Tipo de recurso plannerAppliedCategories
description: O **recurso AppliedCategoriesCollection** representa a coleção de categorias (ou rótulos) que foram aplicadas a uma tarefa. Ele faz parte do objeto plannerTask.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: 1a7513ed9746cb73a08882f3b9c9167ef5336e281bf21fa7f359c80541232c81
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54246651"
---
# <a name="plannerappliedcategories-resource-type"></a>Tipo de recurso plannerAppliedCategories

Namespace: microsoft.graph


O **recurso AppliedCategoriesCollection** representa a coleção de categorias (ou rótulos) que foram aplicadas a uma tarefa. Ele faz parte do [objeto plannerTask.](plannertask.md)
Pode haver até 6 categorias aplicadas a uma tarefa. Descrições de categoria, por `category1` exemplo, , `category2` etc., fazem parte do objeto de detalhes [do](plannerplandetails.md) plano. Esse é um tipo aberto.

## <a name="properties"></a>Propriedades
As propriedades de um Tipo Aberto podem ser definidas pelo cliente. Nesse caso, porém, o cliente deve fornecer , , , , e/ou como propriedades com seus valores sendo o booleano quando as categorias correspondentes são `category1` `category2` `category3` `category4` `category5` `category6` `true` aplicadas à tarefa. Exemplo é mostrado abaixo. Quando não se aplicam, as propriedades são removidas automaticamente definindo seus valores como `false` booleano. 

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

