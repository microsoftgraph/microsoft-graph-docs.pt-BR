---
title: tipo de recurso plannerAppliedCategories
description: O recurso **AppliedCategoriesCollection** representa a coleção de categorias (ou rótulos) que foram aplicados a uma tarefa. Ele faz parte do objeto plannerTask.
localization_priority: Normal
author: TarkanSevilmis
ms.prod: planner
ms.openlocfilehash: b4e3ae92d179669d449d33c34ade4ae4476570fa
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541343"
---
# <a name="plannerappliedcategories-resource-type"></a><span data-ttu-id="f4fde-104">tipo de recurso plannerAppliedCategories</span><span class="sxs-lookup"><span data-stu-id="f4fde-104">plannerAppliedCategories resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4fde-105">O recurso **AppliedCategoriesCollection** representa a coleção de categorias (ou rótulos) que foram aplicados a uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="f4fde-105">The **AppliedCategoriesCollection** resource represents the collection of categories (or labels) that have been applied to a task.</span></span> <span data-ttu-id="f4fde-106">Ele faz parte do objeto [plannerTask](plannertask.md) .</span><span class="sxs-lookup"><span data-stu-id="f4fde-106">It is part of the [plannerTask](plannertask.md) object.</span></span>
<span data-ttu-id="f4fde-107">Pode haver até 6 categorias aplicadas a uma tarefa.</span><span class="sxs-lookup"><span data-stu-id="f4fde-107">There can be up to 6 categories applied to a task.</span></span> <span data-ttu-id="f4fde-108">Descrições de categoria, por `category1`exemplo `category2` , etc., fazem parte do objeto [Plan Details](plannerplandetails.md) .</span><span class="sxs-lookup"><span data-stu-id="f4fde-108">Category descriptions, e.g. `category1`, `category2` etc., are part of the [plan details](plannerplandetails.md) object.</span></span> <span data-ttu-id="f4fde-109">Este é um tipo aberto.</span><span class="sxs-lookup"><span data-stu-id="f4fde-109">This is an open type.</span></span>

## <a name="properties"></a><span data-ttu-id="f4fde-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f4fde-110">Properties</span></span>
<span data-ttu-id="f4fde-111">As propriedades de um tipo aberto podem ser definidas pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f4fde-111">Properties of an Open Type can be defined by the client.</span></span> <span data-ttu-id="f4fde-112">Nesse caso, no entanto, o cliente `category1`deve `category2`fornecer `category3`, `category4`, `category5` , e/ `category6` ou como propriedades com seus valores sendo `true` Boolean quando as categorias correspondentes são aplicadas à tarefa.</span><span class="sxs-lookup"><span data-stu-id="f4fde-112">In this case though, the client must provide `category1`, `category2`, `category3`, `category4`, `category5` and/or `category6` as properties with their values being the `true` boolean when the corresponding categories are applied on the task.</span></span> <span data-ttu-id="f4fde-113">O exemplo é mostrado abaixo.</span><span class="sxs-lookup"><span data-stu-id="f4fde-113">Example is shown below.</span></span> <span data-ttu-id="f4fde-114">Quando eles não se aplicam, as propriedades são removidas automaticamente definindo seus `false` valores para o Boolean.</span><span class="sxs-lookup"><span data-stu-id="f4fde-114">When they do not apply, properties are automatically removed by setting their values to the `false` boolean.</span></span> 

## <a name="json-representation"></a><span data-ttu-id="f4fde-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f4fde-115">JSON representation</span></span>

<span data-ttu-id="f4fde-116">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="f4fde-116">Here is a JSON representation of the resource</span></span>

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

<span data-ttu-id="f4fde-117">Exemplo:</span><span class="sxs-lookup"><span data-stu-id="f4fde-117">Example:</span></span> 

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
