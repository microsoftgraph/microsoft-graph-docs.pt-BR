---
title: Tipo de recurso Filter
description: Gerencia a filtragem da coluna de uma tabela.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 3f58e1f5207fc3b4aebe2fdfb780735c0c5d209d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032477"
---
# <a name="filter-resource-type"></a><span data-ttu-id="9c071-103">Tipo de recurso Filter</span><span class="sxs-lookup"><span data-stu-id="9c071-103">Filter resource type</span></span>

<span data-ttu-id="9c071-104">Gerencia a filtragem da coluna de uma tabela.</span><span class="sxs-lookup"><span data-stu-id="9c071-104">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="9c071-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="9c071-105">Methods</span></span>

| <span data-ttu-id="9c071-106">Método</span><span class="sxs-lookup"><span data-stu-id="9c071-106">Method</span></span>           | <span data-ttu-id="9c071-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9c071-107">Return Type</span></span>    |<span data-ttu-id="9c071-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c071-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9c071-109">Apply</span><span class="sxs-lookup"><span data-stu-id="9c071-109">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="9c071-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9c071-110">None</span></span>|<span data-ttu-id="9c071-111">Aplica os critérios de filtro determinados à coluna fornecida.</span><span class="sxs-lookup"><span data-stu-id="9c071-111">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="9c071-112">Clear</span><span class="sxs-lookup"><span data-stu-id="9c071-112">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="9c071-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9c071-113">None</span></span>|<span data-ttu-id="9c071-114">Limpa o filtro na coluna determinada.</span><span class="sxs-lookup"><span data-stu-id="9c071-114">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="9c071-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9c071-115">Properties</span></span>

| <span data-ttu-id="9c071-116">Nome</span><span class="sxs-lookup"><span data-stu-id="9c071-116">Name</span></span> | <span data-ttu-id="9c071-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="9c071-117">Type</span></span>   |<span data-ttu-id="9c071-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="9c071-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9c071-119">criteria</span><span class="sxs-lookup"><span data-stu-id="9c071-119">criteria</span></span>|[<span data-ttu-id="9c071-120">WorkbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="9c071-120">WorkbookFilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="9c071-121">O filtro aplicado no momento à coluna fornecida.</span><span class="sxs-lookup"><span data-stu-id="9c071-121">The currently applied filter on the given column.</span></span> <span data-ttu-id="9c071-122">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9c071-122">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9c071-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9c071-123">JSON representation</span></span>

<span data-ttu-id="9c071-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9c071-124">Here is a JSON representation of the resource.</span></span>

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
