---
title: tipo de recurso workbookFilter
description: Gerencia a filtragem da coluna de uma tabela.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: excel
author: ruoyingl
ms.openlocfilehash: 39ebe2f59e5741e4580ef5300400a0b7e480ffad
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808513"
---
# <a name="workbookfilter-resource-type"></a><span data-ttu-id="46115-103">tipo de recurso workbookFilter</span><span class="sxs-lookup"><span data-stu-id="46115-103">workbookFilter resource type</span></span>

<span data-ttu-id="46115-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46115-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="46115-105">Gerencia a filtragem da coluna de uma tabela.</span><span class="sxs-lookup"><span data-stu-id="46115-105">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="46115-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="46115-106">Methods</span></span>

| <span data-ttu-id="46115-107">Método</span><span class="sxs-lookup"><span data-stu-id="46115-107">Method</span></span>           | <span data-ttu-id="46115-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="46115-108">Return Type</span></span>    |<span data-ttu-id="46115-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="46115-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="46115-110">Apply</span><span class="sxs-lookup"><span data-stu-id="46115-110">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="46115-111">Nenhum</span><span class="sxs-lookup"><span data-stu-id="46115-111">None</span></span>|<span data-ttu-id="46115-112">Aplica os critérios de filtro determinados à coluna fornecida.</span><span class="sxs-lookup"><span data-stu-id="46115-112">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="46115-113">Clear</span><span class="sxs-lookup"><span data-stu-id="46115-113">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="46115-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="46115-114">None</span></span>|<span data-ttu-id="46115-115">Limpa o filtro na coluna determinada.</span><span class="sxs-lookup"><span data-stu-id="46115-115">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="46115-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="46115-116">Properties</span></span>
<span data-ttu-id="46115-117">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="46115-117">None</span></span>

## <a name="relationships"></a><span data-ttu-id="46115-118">Relações</span><span class="sxs-lookup"><span data-stu-id="46115-118">Relationships</span></span>
| <span data-ttu-id="46115-119">Relação</span><span class="sxs-lookup"><span data-stu-id="46115-119">Relationship</span></span> | <span data-ttu-id="46115-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="46115-120">Type</span></span>   |<span data-ttu-id="46115-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="46115-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="46115-122">criteria</span><span class="sxs-lookup"><span data-stu-id="46115-122">criteria</span></span>|[<span data-ttu-id="46115-123">workbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="46115-123">workbookFilterCriteria</span></span>](workbookfiltercriteria.md)|<span data-ttu-id="46115-124">O filtro aplicado no momento à coluna fornecida.</span><span class="sxs-lookup"><span data-stu-id="46115-124">The currently applied filter on the given column.</span></span> <span data-ttu-id="46115-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="46115-125">Read-only.</span></span>|


## <a name="json-representation"></a><span data-ttu-id="46115-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="46115-126">JSON representation</span></span>

<span data-ttu-id="46115-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="46115-127">Here is a JSON representation of the resource.</span></span>

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
