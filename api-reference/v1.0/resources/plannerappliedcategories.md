---
title: tipo de recurso plannerAppliedCategories
description: O recurso **AppliedCategoriesCollection** representa a coleção de categorias (ou rótulos) que foram aplicados a uma tarefa. Ele faz parte do objeto plannerTask.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
doc_type: resourcePageType
ms.openlocfilehash: fac4c69e9827e903d18f8665bc9b33e7c32705e2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48037623"
---
# <a name="plannerappliedcategories-resource-type"></a><span data-ttu-id="93ae1-104">tipo de recurso plannerAppliedCategories</span><span class="sxs-lookup"><span data-stu-id="93ae1-104">plannerAppliedCategories resource type</span></span>

<span data-ttu-id="93ae1-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93ae1-105">Namespace: microsoft.graph</span></span>


<span data-ttu-id="93ae1-106">O recurso **AppliedCategoriesCollection** representa a coleção de categorias (ou rótulos) que foram aplicados a uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="93ae1-106">The **AppliedCategoriesCollection** resource represents the collection of categories (or labels) that have been applied to a task.</span></span> <span data-ttu-id="93ae1-107">Ele faz parte do objeto [plannerTask](plannertask.md) .</span><span class="sxs-lookup"><span data-stu-id="93ae1-107">It is part of the [plannerTask](plannertask.md) object.</span></span>
<span data-ttu-id="93ae1-108">Pode haver até 6 categorias aplicadas a uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="93ae1-108">There can be up to 6 categories applied to a task.</span></span> <span data-ttu-id="93ae1-109">Descrições de categoria, por exemplo, `category1` `category2` etc., fazem parte do objeto [Plan Details](plannerplandetails.md) .</span><span class="sxs-lookup"><span data-stu-id="93ae1-109">Category descriptions, e.g. `category1`, `category2` etc., are part of the [plan details](plannerplandetails.md) object.</span></span> <span data-ttu-id="93ae1-110">Este é um tipo aberto.</span><span class="sxs-lookup"><span data-stu-id="93ae1-110">This is an open type.</span></span>

## <a name="properties"></a><span data-ttu-id="93ae1-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="93ae1-111">Properties</span></span>
<span data-ttu-id="93ae1-112">As propriedades de um tipo aberto podem ser definidas pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="93ae1-112">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="93ae1-113">Nesse caso, no entanto, o cliente deve fornecer,,, `category1` `category2` `category3` `category4` `category5` e/ou `category6` como propriedades com seus valores sendo `true` Boolean quando as categorias correspondentes são aplicadas à tarefa.</span><span class="sxs-lookup"><span data-stu-id="93ae1-113">In this case though, the client must provide `category1`, `category2`, `category3`, `category4`, `category5` and/or `category6` as properties with their values being the `true` boolean when the corresponding categories are applied on the task.</span></span> <span data-ttu-id="93ae1-114">O exemplo é mostrado abaixo.</span><span class="sxs-lookup"><span data-stu-id="93ae1-114">Example is shown below.</span></span> <span data-ttu-id="93ae1-115">Quando eles não se aplicam, as propriedades são removidas automaticamente definindo seus valores para o `false` Boolean.</span><span class="sxs-lookup"><span data-stu-id="93ae1-115">When they do not apply, properties are automatically removed by setting their values to the `false` boolean.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="93ae1-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="93ae1-116">JSON representation</span></span>

<span data-ttu-id="93ae1-117">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="93ae1-117">Here is a JSON representation of the resource</span></span>

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

<span data-ttu-id="93ae1-118">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="93ae1-118">Example:</span></span> 

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

