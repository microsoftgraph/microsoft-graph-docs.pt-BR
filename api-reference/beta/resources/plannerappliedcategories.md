---
title: Tipo de recurso plannerAppliedCategories
description: O recurso de **AppliedCategoriesCollection** representa a coleção de categorias (ou rótulos) que tiverem sido aplicadas a uma tarefa. Ele faz parte do objeto plannerTask.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: b4e3ae92d179669d449d33c34ade4ae4476570fa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517663"
---
# <a name="plannerappliedcategories-resource-type"></a><span data-ttu-id="bd2f7-104">Tipo de recurso plannerAppliedCategories</span><span class="sxs-lookup"><span data-stu-id="bd2f7-104">plannerAppliedCategories resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bd2f7-p102">O recurso **AppliedCategoriesCollection** representa a coleção de categorias (ou rótulos) que foram aplicadas a uma tarefa. Ele faz parte do objeto [plannerTask](plannertask.md). Pode haver até seis categorias aplicadas a uma tarefa. Descrições de categorias, por exemplo, `category1`, `category2` etc., fazem parte do objeto [plan details](plannerplandetails.md). Este é um Tipo Aberto.</span><span class="sxs-lookup"><span data-stu-id="bd2f7-p102">The **AppliedCategoriesCollection** resource represents the collection of categories (or labels) that have been applied to a task. It is part of the [plannerTask](plannertask.md) object. There can be up to 6 categories applied to a task. Category descriptions, e.g. `category1`, `category2` etc., are part of the [plan details](plannerplandetails.md) object. This is an open type.</span></span>

## <a name="properties"></a><span data-ttu-id="bd2f7-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bd2f7-110">Properties</span></span>
<span data-ttu-id="bd2f7-p103">As propriedades de um Tipo Aberto podem ser definidas pelo cliente. Nesse caso, o cliente deve fornecer `category1`, `category2`, `category3`, `category4`, `category5` e/ou `category6` como propriedades com seus valores representados pelo booliano `true` quando as categorias correspondentes são aplicadas à tarefa. Um exemplo é mostrado abaixo. Quando elas não se aplicam, as propriedades são automaticamente removidas ao configurar os valores com o booliano `false`.</span><span class="sxs-lookup"><span data-stu-id="bd2f7-p103">Properties of an Open Type can be defined by the client. In this case though, the client must provide `category1`, `category2`, `category3`, `category4`, `category5` and/or `category6` as properties with their values being the `true` boolean when the corresponding categories are applied on the task. Example is shown below. When they do not apply, properties are automatically removed by setting their values to the `false` boolean.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="bd2f7-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bd2f7-115">JSON representation</span></span>

<span data-ttu-id="bd2f7-116">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="bd2f7-116">Here is a JSON representation of the resource</span></span>

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

<span data-ttu-id="bd2f7-117">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="bd2f7-117">Example:</span></span> 

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
  "suppressions": [
    "Error: /api-reference/beta/resources/plannerappliedcategories.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
