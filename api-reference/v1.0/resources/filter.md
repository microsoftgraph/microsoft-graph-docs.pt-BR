---
title: Tipo de recurso Filter
description: Gerencia a filtragem da coluna de uma tabela.
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 06167bbb0eb55da409e807aeabc9bfaf8287cc9b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531416"
---
# <a name="filter-resource-type"></a><span data-ttu-id="002cd-103">Tipo de recurso Filter</span><span class="sxs-lookup"><span data-stu-id="002cd-103">Filter resource type</span></span>

<span data-ttu-id="002cd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="002cd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="002cd-105">Gerencia a filtragem da coluna de uma tabela.</span><span class="sxs-lookup"><span data-stu-id="002cd-105">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="002cd-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="002cd-106">Methods</span></span>

| <span data-ttu-id="002cd-107">Método</span><span class="sxs-lookup"><span data-stu-id="002cd-107">Method</span></span>           | <span data-ttu-id="002cd-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="002cd-108">Return Type</span></span>    |<span data-ttu-id="002cd-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="002cd-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="002cd-110">Apply</span><span class="sxs-lookup"><span data-stu-id="002cd-110">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="002cd-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="002cd-111">None</span></span>|<span data-ttu-id="002cd-112">Aplica os critérios de filtro determinados à coluna fornecida.</span><span class="sxs-lookup"><span data-stu-id="002cd-112">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="002cd-113">Clear</span><span class="sxs-lookup"><span data-stu-id="002cd-113">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="002cd-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="002cd-114">None</span></span>|<span data-ttu-id="002cd-115">Limpa o filtro na coluna determinada.</span><span class="sxs-lookup"><span data-stu-id="002cd-115">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="002cd-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="002cd-116">Properties</span></span>

| <span data-ttu-id="002cd-117">Nome</span><span class="sxs-lookup"><span data-stu-id="002cd-117">Name</span></span> | <span data-ttu-id="002cd-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="002cd-118">Type</span></span>   |<span data-ttu-id="002cd-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="002cd-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="002cd-120">criteria</span><span class="sxs-lookup"><span data-stu-id="002cd-120">criteria</span></span>|[<span data-ttu-id="002cd-121">WorkbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="002cd-121">WorkbookFilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="002cd-122">O filtro aplicado no momento à coluna fornecida.</span><span class="sxs-lookup"><span data-stu-id="002cd-122">The currently applied filter on the given column.</span></span> <span data-ttu-id="002cd-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="002cd-123">Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="002cd-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="002cd-124">JSON representation</span></span>

<span data-ttu-id="002cd-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="002cd-125">Here is a JSON representation of the resource.</span></span>

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
