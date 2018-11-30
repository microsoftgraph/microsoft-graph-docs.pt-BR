---
title: Tipo de recurso Filter
description: Gerencia a filtragem da coluna de uma tabela.
ms.openlocfilehash: df896d10b1e8734015d38b92b5824e3e3652e3a6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037734"
---
# <a name="filter-resource-type"></a><span data-ttu-id="94736-103">Tipo de recurso Filter</span><span class="sxs-lookup"><span data-stu-id="94736-103">Filter resource type</span></span>

> <span data-ttu-id="94736-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="94736-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94736-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="94736-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="94736-106">Gerencia a filtragem da coluna de uma tabela.</span><span class="sxs-lookup"><span data-stu-id="94736-106">Manages the filtering of a table's column.</span></span>


## <a name="methods"></a><span data-ttu-id="94736-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="94736-107">Methods</span></span>

| <span data-ttu-id="94736-108">Método</span><span class="sxs-lookup"><span data-stu-id="94736-108">Method</span></span>           | <span data-ttu-id="94736-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="94736-109">Return Type</span></span>    |<span data-ttu-id="94736-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="94736-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="94736-111">Aplicar</span><span class="sxs-lookup"><span data-stu-id="94736-111">Apply</span></span>](../api/filter-apply.md)|<span data-ttu-id="94736-112">Nenhum</span><span class="sxs-lookup"><span data-stu-id="94736-112">None</span></span>|<span data-ttu-id="94736-113">Aplica os critérios de filtro determinados à coluna fornecida.</span><span class="sxs-lookup"><span data-stu-id="94736-113">Apply the given filter criteria on the given column.</span></span>|
|[<span data-ttu-id="94736-114">Clear</span><span class="sxs-lookup"><span data-stu-id="94736-114">Clear</span></span>](../api/filter-clear.md)|<span data-ttu-id="94736-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="94736-115">None</span></span>|<span data-ttu-id="94736-116">Limpa o filtro na coluna determinada.</span><span class="sxs-lookup"><span data-stu-id="94736-116">Clear the filter on the given column.</span></span>|

## <a name="properties"></a><span data-ttu-id="94736-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="94736-117">Properties</span></span>
<span data-ttu-id="94736-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="94736-118">None</span></span>

## <a name="relationships"></a><span data-ttu-id="94736-119">Relações</span><span class="sxs-lookup"><span data-stu-id="94736-119">Relationships</span></span>
| <span data-ttu-id="94736-120">Relação</span><span class="sxs-lookup"><span data-stu-id="94736-120">Relationship</span></span> | <span data-ttu-id="94736-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="94736-121">Type</span></span>   |<span data-ttu-id="94736-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="94736-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94736-123">critérios</span><span class="sxs-lookup"><span data-stu-id="94736-123">criteria</span></span>|[<span data-ttu-id="94736-124">FilterCriteria</span><span class="sxs-lookup"><span data-stu-id="94736-124">FilterCriteria</span></span>](filtercriteria.md)|<span data-ttu-id="94736-p102">O filtro aplicado no momento à coluna fornecida. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="94736-p102">The currently applied filter on the given column. Read-only.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Filter resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->