---
title: Tipo de recurso Filter
description: Gerencia a filtragem da coluna de uma tabela.
localization_priority: Normal
ms.openlocfilehash: 6adc4e378b47bcb134a640e77bf54c32a35b3be2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518888"
---
# <a name="filter-resource-type"></a><span data-ttu-id="65099-103">Tipo de recurso Filter</span><span class="sxs-lookup"><span data-stu-id="65099-103">Filter resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65099-104">Gerencia a filtragem da coluna de uma tabela.</span><span class="sxs-lookup"><span data-stu-id="65099-104">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="65099-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="65099-105">Methods</span></span>

| <span data-ttu-id="65099-106">Método</span><span class="sxs-lookup"><span data-stu-id="65099-106">Method</span></span>           | <span data-ttu-id="65099-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="65099-107">Return Type</span></span>    |<span data-ttu-id="65099-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="65099-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="65099-109">Aplicar</span><span class="sxs-lookup"><span data-stu-id="65099-109">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="65099-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="65099-110">None</span></span>|<span data-ttu-id="65099-111">Aplica os critérios de filtro determinados à coluna fornecida.</span><span class="sxs-lookup"><span data-stu-id="65099-111">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="65099-112">Clear</span><span class="sxs-lookup"><span data-stu-id="65099-112">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="65099-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="65099-113">None</span></span>|<span data-ttu-id="65099-114">Limpa o filtro na coluna determinada.</span><span class="sxs-lookup"><span data-stu-id="65099-114">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="65099-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="65099-115">Properties</span></span>
<span data-ttu-id="65099-116">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="65099-116">None</span></span>

## <a name="relationships"></a><span data-ttu-id="65099-117">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="65099-117">Relationships</span></span>
| <span data-ttu-id="65099-118">Relação</span><span class="sxs-lookup"><span data-stu-id="65099-118">Relationship</span></span> | <span data-ttu-id="65099-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="65099-119">Type</span></span>   |<span data-ttu-id="65099-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="65099-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="65099-121">critérios</span><span class="sxs-lookup"><span data-stu-id="65099-121">criteria</span></span>|[<span data-ttu-id="65099-122">FilterCriteria</span><span class="sxs-lookup"><span data-stu-id="65099-122">FilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="65099-p101">O filtro aplicado no momento à coluna fornecida. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="65099-p101">The currently applied filter on the given column. Read-only.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/filter.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
