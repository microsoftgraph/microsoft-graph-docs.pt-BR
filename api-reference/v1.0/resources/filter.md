---
title: Tipo de recurso Filter
description: Gerencia a filtragem da coluna de uma tabela.
localization_priority: Normal
author: ruoyingl
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c85c8237f179fd6be2add02263c9d6d040a71849
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018302"
---
# <a name="filter-resource-type"></a><span data-ttu-id="bfb6d-103">Tipo de recurso Filter</span><span class="sxs-lookup"><span data-stu-id="bfb6d-103">Filter resource type</span></span>

<span data-ttu-id="bfb6d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bfb6d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="bfb6d-105">Gerencia a filtragem da coluna de uma tabela.</span><span class="sxs-lookup"><span data-stu-id="bfb6d-105">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="bfb6d-106">Methods</span><span class="sxs-lookup"><span data-stu-id="bfb6d-106">Methods</span></span>

| <span data-ttu-id="bfb6d-107">Método</span><span class="sxs-lookup"><span data-stu-id="bfb6d-107">Method</span></span>           | <span data-ttu-id="bfb6d-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bfb6d-108">Return Type</span></span>    |<span data-ttu-id="bfb6d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfb6d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bfb6d-110">Apply</span><span class="sxs-lookup"><span data-stu-id="bfb6d-110">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="bfb6d-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bfb6d-111">None</span></span>|<span data-ttu-id="bfb6d-112">Aplica os critérios de filtro determinados à coluna fornecida.</span><span class="sxs-lookup"><span data-stu-id="bfb6d-112">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="bfb6d-113">Clear</span><span class="sxs-lookup"><span data-stu-id="bfb6d-113">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="bfb6d-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bfb6d-114">None</span></span>|<span data-ttu-id="bfb6d-115">Limpa o filtro na coluna determinada.</span><span class="sxs-lookup"><span data-stu-id="bfb6d-115">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="bfb6d-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bfb6d-116">Properties</span></span>

| <span data-ttu-id="bfb6d-117">Nome</span><span class="sxs-lookup"><span data-stu-id="bfb6d-117">Name</span></span> | <span data-ttu-id="bfb6d-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="bfb6d-118">Type</span></span>   |<span data-ttu-id="bfb6d-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="bfb6d-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bfb6d-120">criteria</span><span class="sxs-lookup"><span data-stu-id="bfb6d-120">criteria</span></span>|[<span data-ttu-id="bfb6d-121">WorkbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="bfb6d-121">WorkbookFilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="bfb6d-122">O filtro aplicado no momento à coluna fornecida.</span><span class="sxs-lookup"><span data-stu-id="bfb6d-122">The currently applied filter on the given column.</span></span> <span data-ttu-id="bfb6d-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="bfb6d-123">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bfb6d-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bfb6d-124">JSON representation</span></span>

<span data-ttu-id="bfb6d-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bfb6d-125">Here is a JSON representation of the resource.</span></span>

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

