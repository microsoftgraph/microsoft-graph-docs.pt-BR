---
title: Tipo de recurso plannerAppliedCategories
description: O recurso de **AppliedCategoriesCollection** representa a coleção de categorias (ou rótulos) que tiverem sido aplicadas a uma tarefa. Ele faz parte do objeto plannerTask.
localization_priority: Normal
ms.openlocfilehash: a47317f907b8ee934a59a320af67e94ce6d3bf8e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27856011"
---
# <a name="plannerappliedcategories-resource-type"></a><span data-ttu-id="bd0b0-104">Tipo de recurso plannerAppliedCategories</span><span class="sxs-lookup"><span data-stu-id="bd0b0-104">plannerAppliedCategories resource type</span></span>

> <span data-ttu-id="bd0b0-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="bd0b0-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bd0b0-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="bd0b0-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bd0b0-p103">O recurso **AppliedCategoriesCollection** representa a coleção de categorias (ou rótulos) que foram aplicadas a uma tarefa. Ele faz parte do objeto [plannerTask](plannertask.md). Pode haver até seis categorias aplicadas a uma tarefa. Descrições de categorias, por exemplo, `category1`, `category2` etc., fazem parte do objeto [plan details](plannerplandetails.md). Este é um Tipo Aberto.</span><span class="sxs-lookup"><span data-stu-id="bd0b0-p103">The **AppliedCategoriesCollection** resource represents the collection of categories (or labels) that have been applied to a task. It is part of the [plannerTask](plannertask.md) object. There can be up to 6 categories applied to a task. Category descriptions, e.g. `category1`, `category2` etc., are part of the [plan details](plannerplandetails.md) object. This is an open type.</span></span>

## <a name="properties"></a><span data-ttu-id="bd0b0-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bd0b0-112">Properties</span></span>
<span data-ttu-id="bd0b0-p104">As propriedades de um Tipo Aberto podem ser definidas pelo cliente. Nesse caso, o cliente deve fornecer `category1`, `category2`, `category3`, `category4`, `category5` e/ou `category6` como propriedades com seus valores representados pelo booliano `true` quando as categorias correspondentes são aplicadas à tarefa. Um exemplo é mostrado abaixo. Quando elas não se aplicam, as propriedades são automaticamente removidas ao configurar os valores com o booliano `false`.</span><span class="sxs-lookup"><span data-stu-id="bd0b0-p104">Properties of an Open Type can be defined by the client. In this case though, the client must provide `category1`, `category2`, `category3`, `category4`, `category5` and/or `category6` as properties with their values being the `true` boolean when the corresponding categories are applied on the task. Example is shown below. When they do not apply, properties are automatically removed by setting their values to the `false` boolean.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="bd0b0-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bd0b0-117">JSON representation</span></span>

<span data-ttu-id="bd0b0-118">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="bd0b0-118">Here is a JSON representation of the resource</span></span>

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

<span data-ttu-id="bd0b0-119">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="bd0b0-119">Example:</span></span> 

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
