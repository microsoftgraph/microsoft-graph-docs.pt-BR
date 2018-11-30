---
title: Tipo de recurso Filter
description: Gerencia a filtragem da coluna de uma tabela.
ms.openlocfilehash: 272b4ea0ee91c25ea845217512a12e33b08ed7b8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27005076"
---
# <a name="filter-resource-type"></a><span data-ttu-id="0cab6-103">Tipo de recurso Filter</span><span class="sxs-lookup"><span data-stu-id="0cab6-103">Filter resource type</span></span>

<span data-ttu-id="0cab6-104">Gerencia a filtragem da coluna de uma tabela.</span><span class="sxs-lookup"><span data-stu-id="0cab6-104">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="0cab6-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="0cab6-105">Methods</span></span>

| <span data-ttu-id="0cab6-106">Método</span><span class="sxs-lookup"><span data-stu-id="0cab6-106">Method</span></span>           | <span data-ttu-id="0cab6-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0cab6-107">Return Type</span></span>    |<span data-ttu-id="0cab6-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cab6-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="0cab6-109">Aplicar</span><span class="sxs-lookup"><span data-stu-id="0cab6-109">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="0cab6-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0cab6-110">None</span></span>|<span data-ttu-id="0cab6-111">Aplica os critérios de filtro determinados à coluna fornecida.</span><span class="sxs-lookup"><span data-stu-id="0cab6-111">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="0cab6-112">Clear</span><span class="sxs-lookup"><span data-stu-id="0cab6-112">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="0cab6-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0cab6-113">None</span></span>|<span data-ttu-id="0cab6-114">Limpa o filtro na coluna determinada.</span><span class="sxs-lookup"><span data-stu-id="0cab6-114">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="0cab6-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0cab6-115">Properties</span></span>

| <span data-ttu-id="0cab6-116">Nome</span><span class="sxs-lookup"><span data-stu-id="0cab6-116">Name</span></span> | <span data-ttu-id="0cab6-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="0cab6-117">Type</span></span>   |<span data-ttu-id="0cab6-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="0cab6-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0cab6-119">critérios</span><span class="sxs-lookup"><span data-stu-id="0cab6-119">criteria</span></span>|[<span data-ttu-id="0cab6-120">WorkbookFilterCriteria</span><span class="sxs-lookup"><span data-stu-id="0cab6-120">WorkbookFilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="0cab6-p101">O filtro aplicado no momento à coluna fornecida. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="0cab6-p101">The currently applied filter on the given column. Read-only.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0cab6-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0cab6-123">JSON representation</span></span>

<span data-ttu-id="0cab6-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0cab6-124">Here is a JSON representation of the resource.</span></span>

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