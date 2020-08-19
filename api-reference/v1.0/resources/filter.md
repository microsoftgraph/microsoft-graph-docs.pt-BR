---
title: Tipo de recurso Filter
description: Gerencia a filtragem da coluna de uma tabela.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: ecaa61bde452d13e7e8e7fe0c79e3b75eeaa591a
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807805"
---
# <a name="filter-resource-type"></a><span data-ttu-id="a8290-103">Tipo de recurso Filter</span><span class="sxs-lookup"><span data-stu-id="a8290-103">Filter resource type</span></span>

<span data-ttu-id="a8290-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a8290-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a8290-105">Gerencia a filtragem da coluna de uma tabela.</span><span class="sxs-lookup"><span data-stu-id="a8290-105">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="a8290-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="a8290-106">Methods</span></span>

| <span data-ttu-id="a8290-107">Método</span><span class="sxs-lookup"><span data-stu-id="a8290-107">Method</span></span>           | <span data-ttu-id="a8290-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a8290-108">Return Type</span></span>    |<span data-ttu-id="a8290-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8290-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a8290-110">Apply</span><span class="sxs-lookup"><span data-stu-id="a8290-110">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="a8290-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a8290-111">None</span></span>|<span data-ttu-id="a8290-112">Aplica os critérios de filtro determinados à coluna fornecida.</span><span class="sxs-lookup"><span data-stu-id="a8290-112">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="a8290-113">Clear</span><span class="sxs-lookup"><span data-stu-id="a8290-113">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="a8290-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a8290-114">None</span></span>|<span data-ttu-id="a8290-115">Limpa o filtro na coluna determinada.</span><span class="sxs-lookup"><span data-stu-id="a8290-115">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="a8290-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a8290-116">Properties</span></span>

| <span data-ttu-id="a8290-117">Nome</span><span class="sxs-lookup"><span data-stu-id="a8290-117">Name</span></span> | <span data-ttu-id="a8290-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="a8290-118">Type</span></span>   |<span data-ttu-id="a8290-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="a8290-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a8290-120">criteria</span><span class="sxs-lookup"><span data-stu-id="a8290-120">criteria</span></span>|[<span data-ttu-id="a8290-121">WorkbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="a8290-121">WorkbookFilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="a8290-122">O filtro aplicado no momento à coluna fornecida.</span><span class="sxs-lookup"><span data-stu-id="a8290-122">The currently applied filter on the given column.</span></span> <span data-ttu-id="a8290-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a8290-123">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a8290-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a8290-124">JSON representation</span></span>

<span data-ttu-id="a8290-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a8290-125">Here is a JSON representation of the resource.</span></span>

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
