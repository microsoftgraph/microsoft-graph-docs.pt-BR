---
title: Tipo de recurso plannerAppliedCategories
description: O recurso de **AppliedCategoriesCollection** representa a coleção de categorias (ou rótulos) que tiverem sido aplicadas a uma tarefa. Ele faz parte do objeto plannerTask.
ms.openlocfilehash: 0bb7987c3da62f2302b08ab43fa00d09763e0c1d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039485"
---
# <a name="plannerappliedcategories-resource-type"></a>Tipo de recurso plannerAppliedCategories

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O recurso **AppliedCategoriesCollection** representa a coleção de categorias (ou rótulos) que foram aplicadas a uma tarefa. Ele faz parte do objeto [plannerTask](plannertask.md). Pode haver até seis categorias aplicadas a uma tarefa. Descrições de categorias, por exemplo, `category1`, `category2` etc., fazem parte do objeto [plan details](plannerplandetails.md). Este é um Tipo Aberto.

## <a name="properties"></a>Propriedades
As propriedades de um Tipo Aberto podem ser definidas pelo cliente. Nesse caso, o cliente deve fornecer `category1`, `category2`, `category3`, `category4`, `category5` e/ou `category6` como propriedades com seus valores representados pelo booliano `true` quando as categorias correspondentes são aplicadas à tarefa. Um exemplo é mostrado abaixo. Quando elas não se aplicam, as propriedades são automaticamente removidas ao configurar os valores com o booliano `false`. 

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
<!-- {
  "type": "#page.annotation",
  "description": "plannerAppliedCategories resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->