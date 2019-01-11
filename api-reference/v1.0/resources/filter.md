---
title: Tipo de recurso Filter
description: Gerencia a filtragem da coluna de uma tabela.
localization_priority: Normal
ms.openlocfilehash: cc4b1b105c2049b36fa27cb88b41102366648fa8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27834661"
---
# <a name="filter-resource-type"></a><span data-ttu-id="ea52a-103">Tipo de recurso Filter</span><span class="sxs-lookup"><span data-stu-id="ea52a-103">Filter resource type</span></span>

<span data-ttu-id="ea52a-104">Gerencia a filtragem da coluna de uma tabela.</span><span class="sxs-lookup"><span data-stu-id="ea52a-104">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="ea52a-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="ea52a-105">Methods</span></span>

| <span data-ttu-id="ea52a-106">Método</span><span class="sxs-lookup"><span data-stu-id="ea52a-106">Method</span></span>           | <span data-ttu-id="ea52a-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ea52a-107">Return Type</span></span>    |<span data-ttu-id="ea52a-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea52a-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ea52a-109">Aplicar</span><span class="sxs-lookup"><span data-stu-id="ea52a-109">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="ea52a-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ea52a-110">None</span></span>|<span data-ttu-id="ea52a-111">Aplica os critérios de filtro determinados à coluna fornecida.</span><span class="sxs-lookup"><span data-stu-id="ea52a-111">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="ea52a-112">Clear</span><span class="sxs-lookup"><span data-stu-id="ea52a-112">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="ea52a-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ea52a-113">None</span></span>|<span data-ttu-id="ea52a-114">Limpa o filtro na coluna determinada.</span><span class="sxs-lookup"><span data-stu-id="ea52a-114">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="ea52a-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ea52a-115">Properties</span></span>

| <span data-ttu-id="ea52a-116">Nome</span><span class="sxs-lookup"><span data-stu-id="ea52a-116">Name</span></span> | <span data-ttu-id="ea52a-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea52a-117">Type</span></span>   |<span data-ttu-id="ea52a-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea52a-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea52a-119">critérios</span><span class="sxs-lookup"><span data-stu-id="ea52a-119">criteria</span></span>|[<span data-ttu-id="ea52a-120">WorkbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="ea52a-120">WorkbookFilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="ea52a-p101">O filtro aplicado no momento à coluna fornecida. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea52a-p101">The currently applied filter on the given column. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ea52a-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea52a-123">JSON representation</span></span>

<span data-ttu-id="ea52a-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ea52a-124">Here is a JSON representation of the resource.</span></span>

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
