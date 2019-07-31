---
title: tipo de recurso workbookFilter
description: Gerencia a filtragem da coluna de uma tabela.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: ''
ms.openlocfilehash: f3622a2efd952907214add4343bb5958adebe606
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007120"
---
# <a name="workbookfilter-resource-type"></a><span data-ttu-id="42092-103">tipo de recurso workbookFilter</span><span class="sxs-lookup"><span data-stu-id="42092-103">workbookFilter resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="42092-104">Gerencia a filtragem da coluna de uma tabela.</span><span class="sxs-lookup"><span data-stu-id="42092-104">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="42092-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="42092-105">Methods</span></span>

| <span data-ttu-id="42092-106">Método</span><span class="sxs-lookup"><span data-stu-id="42092-106">Method</span></span>           | <span data-ttu-id="42092-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="42092-107">Return Type</span></span>    |<span data-ttu-id="42092-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="42092-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="42092-109">Apply</span><span class="sxs-lookup"><span data-stu-id="42092-109">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="42092-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="42092-110">None</span></span>|<span data-ttu-id="42092-111">Aplica os critérios de filtro determinados à coluna fornecida.</span><span class="sxs-lookup"><span data-stu-id="42092-111">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="42092-112">Clear</span><span class="sxs-lookup"><span data-stu-id="42092-112">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="42092-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="42092-113">None</span></span>|<span data-ttu-id="42092-114">Limpa o filtro na coluna determinada.</span><span class="sxs-lookup"><span data-stu-id="42092-114">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="42092-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="42092-115">Properties</span></span>
<span data-ttu-id="42092-116">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="42092-116">None</span></span>

## <a name="relationships"></a><span data-ttu-id="42092-117">Relações</span><span class="sxs-lookup"><span data-stu-id="42092-117">Relationships</span></span>
| <span data-ttu-id="42092-118">Relação</span><span class="sxs-lookup"><span data-stu-id="42092-118">Relationship</span></span> | <span data-ttu-id="42092-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="42092-119">Type</span></span>   |<span data-ttu-id="42092-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="42092-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42092-121">criteria</span><span class="sxs-lookup"><span data-stu-id="42092-121">criteria</span></span>|[<span data-ttu-id="42092-122">workbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="42092-122">workbookFilterCriteria</span></span>](workbookfiltercriteria.md)|<span data-ttu-id="42092-123">O filtro aplicado no momento à coluna fornecida.</span><span class="sxs-lookup"><span data-stu-id="42092-123">The currently applied filter on the given column.</span></span> <span data-ttu-id="42092-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="42092-124">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="42092-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="42092-125">JSON representation</span></span>

<span data-ttu-id="42092-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="42092-126">Here is a JSON representation of the resource.</span></span>

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
