---
title: Tipo de recurso Filter
description: Gerencia a filtragem da coluna de uma tabela.
localization_priority: Normal
ms.openlocfilehash: 6adc4e378b47bcb134a640e77bf54c32a35b3be2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506404"
---
# <a name="filter-resource-type"></a><span data-ttu-id="ff94f-103">Tipo de recurso Filter</span><span class="sxs-lookup"><span data-stu-id="ff94f-103">Filter resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff94f-104">Gerencia a filtragem da coluna de uma tabela.</span><span class="sxs-lookup"><span data-stu-id="ff94f-104">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="ff94f-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="ff94f-105">Methods</span></span>

| <span data-ttu-id="ff94f-106">Método</span><span class="sxs-lookup"><span data-stu-id="ff94f-106">Method</span></span>           | <span data-ttu-id="ff94f-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ff94f-107">Return Type</span></span>    |<span data-ttu-id="ff94f-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff94f-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ff94f-109">Apply</span><span class="sxs-lookup"><span data-stu-id="ff94f-109">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="ff94f-110">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ff94f-110">None</span></span>|<span data-ttu-id="ff94f-111">Aplica os critérios de filtro determinados à coluna fornecida.</span><span class="sxs-lookup"><span data-stu-id="ff94f-111">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="ff94f-112">Clear</span><span class="sxs-lookup"><span data-stu-id="ff94f-112">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="ff94f-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ff94f-113">None</span></span>|<span data-ttu-id="ff94f-114">Limpa o filtro na coluna determinada.</span><span class="sxs-lookup"><span data-stu-id="ff94f-114">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="ff94f-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ff94f-115">Properties</span></span>
<span data-ttu-id="ff94f-116">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="ff94f-116">None</span></span>

## <a name="relationships"></a><span data-ttu-id="ff94f-117">Relações</span><span class="sxs-lookup"><span data-stu-id="ff94f-117">Relationships</span></span>
| <span data-ttu-id="ff94f-118">Relação</span><span class="sxs-lookup"><span data-stu-id="ff94f-118">Relationship</span></span> | <span data-ttu-id="ff94f-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff94f-119">Type</span></span>   |<span data-ttu-id="ff94f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff94f-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff94f-121">criteria</span><span class="sxs-lookup"><span data-stu-id="ff94f-121">criteria</span></span>|[<span data-ttu-id="ff94f-122">FilterCriteria</span><span class="sxs-lookup"><span data-stu-id="ff94f-122">FilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="ff94f-p101">O filtro aplicado no momento à coluna fornecida. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ff94f-p101">The currently applied filter on the given column. Read-only.</span></span>|

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
