---
title: tipo de recurso workbookFilter
description: Gerencia a filtragem da coluna de uma tabela.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: ''
ms.openlocfilehash: 4a6255f522955e7e2041a8b9b2b23e39c5379ea1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42519229"
---
# <a name="workbookfilter-resource-type"></a><span data-ttu-id="69131-103">tipo de recurso workbookFilter</span><span class="sxs-lookup"><span data-stu-id="69131-103">workbookFilter resource type</span></span>

<span data-ttu-id="69131-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="69131-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69131-105">Gerencia a filtragem da coluna de uma tabela.</span><span class="sxs-lookup"><span data-stu-id="69131-105">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="69131-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="69131-106">Methods</span></span>

| <span data-ttu-id="69131-107">Método</span><span class="sxs-lookup"><span data-stu-id="69131-107">Method</span></span>           | <span data-ttu-id="69131-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="69131-108">Return Type</span></span>    |<span data-ttu-id="69131-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="69131-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="69131-110">Apply</span><span class="sxs-lookup"><span data-stu-id="69131-110">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="69131-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="69131-111">None</span></span>|<span data-ttu-id="69131-112">Aplica os critérios de filtro determinados à coluna fornecida.</span><span class="sxs-lookup"><span data-stu-id="69131-112">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="69131-113">Clear</span><span class="sxs-lookup"><span data-stu-id="69131-113">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="69131-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="69131-114">None</span></span>|<span data-ttu-id="69131-115">Limpa o filtro na coluna determinada.</span><span class="sxs-lookup"><span data-stu-id="69131-115">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="69131-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="69131-116">Properties</span></span>
<span data-ttu-id="69131-117">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="69131-117">None</span></span>

## <a name="relationships"></a><span data-ttu-id="69131-118">Relações</span><span class="sxs-lookup"><span data-stu-id="69131-118">Relationships</span></span>
| <span data-ttu-id="69131-119">Relação</span><span class="sxs-lookup"><span data-stu-id="69131-119">Relationship</span></span> | <span data-ttu-id="69131-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="69131-120">Type</span></span>   |<span data-ttu-id="69131-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="69131-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="69131-122">criteria</span><span class="sxs-lookup"><span data-stu-id="69131-122">criteria</span></span>|[<span data-ttu-id="69131-123">workbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="69131-123">workbookFilterCriteria</span></span>](workbookfiltercriteria.md)|<span data-ttu-id="69131-124">O filtro aplicado no momento à coluna fornecida.</span><span class="sxs-lookup"><span data-stu-id="69131-124">The currently applied filter on the given column.</span></span> <span data-ttu-id="69131-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="69131-125">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="69131-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="69131-126">JSON representation</span></span>

<span data-ttu-id="69131-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="69131-127">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
     "legacyId"
  ],
  "keyProperty": "id",
  "baseType":"microsoft.graph.entity",
  "@odata.type": "microsoft.graph.workbookFilter"
}-->

```json
{
    "criteria": {"@odata.type": "microsoft.graph.workbookFilterCriteria"}
}

```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
