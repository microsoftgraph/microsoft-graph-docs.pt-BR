---
title: Tipo de recurso Filter
description: Gerencia a filtragem da coluna de uma tabela.
localization_priority: Normal
ms.openlocfilehash: cc4b1b105c2049b36fa27cb88b41102366648fa8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564313"
---
# <a name="filter-resource-type"></a><span data-ttu-id="ae448-103">Tipo de recurso Filter</span><span class="sxs-lookup"><span data-stu-id="ae448-103">Filter resource type</span></span>

<span data-ttu-id="ae448-104">Gerencia a filtragem da coluna de uma tabela.</span><span class="sxs-lookup"><span data-stu-id="ae448-104">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="ae448-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="ae448-105">Methods</span></span>

| <span data-ttu-id="ae448-106">Método</span><span class="sxs-lookup"><span data-stu-id="ae448-106">Method</span></span>           | <span data-ttu-id="ae448-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ae448-107">Return Type</span></span>    |<span data-ttu-id="ae448-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae448-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ae448-109">Apply</span><span class="sxs-lookup"><span data-stu-id="ae448-109">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="ae448-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ae448-110">None</span></span>|<span data-ttu-id="ae448-111">Aplica os critérios de filtro determinados à coluna fornecida.</span><span class="sxs-lookup"><span data-stu-id="ae448-111">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="ae448-112">Clear</span><span class="sxs-lookup"><span data-stu-id="ae448-112">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="ae448-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ae448-113">None</span></span>|<span data-ttu-id="ae448-114">Limpa o filtro na coluna determinada.</span><span class="sxs-lookup"><span data-stu-id="ae448-114">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="ae448-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ae448-115">Properties</span></span>

| <span data-ttu-id="ae448-116">Nome</span><span class="sxs-lookup"><span data-stu-id="ae448-116">Name</span></span> | <span data-ttu-id="ae448-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="ae448-117">Type</span></span>   |<span data-ttu-id="ae448-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="ae448-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ae448-119">criteria</span><span class="sxs-lookup"><span data-stu-id="ae448-119">criteria</span></span>|[<span data-ttu-id="ae448-120">WorkbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="ae448-120">WorkbookFilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="ae448-121">O filtro aplicado no momento à coluna fornecida.</span><span class="sxs-lookup"><span data-stu-id="ae448-121">The currently applied filter on the given column.</span></span> <span data-ttu-id="ae448-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ae448-122">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ae448-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ae448-123">JSON representation</span></span>

<span data-ttu-id="ae448-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ae448-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookFilter"
}-->

```json
{
  "criteria": {"@odata.type": "microsoft.graph.workbookFilterCriteria" }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
