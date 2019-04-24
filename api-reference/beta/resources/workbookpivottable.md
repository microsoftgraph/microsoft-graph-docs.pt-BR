---
title: tipo de recurso de tabela dinâmica
description: Representa uma Tabela Dinâmica do Excel.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: fc43bf160e93e354ff58b2f960e8ec38d252287f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32453874"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="ea2af-103">tipo de recurso de tabela dinâmica</span><span class="sxs-lookup"><span data-stu-id="ea2af-103">pivotTable resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea2af-104">Representa uma Tabela Dinâmica do Excel.</span><span class="sxs-lookup"><span data-stu-id="ea2af-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="ea2af-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="ea2af-105">Methods</span></span>

| <span data-ttu-id="ea2af-106">Método</span><span class="sxs-lookup"><span data-stu-id="ea2af-106">Method</span></span>           | <span data-ttu-id="ea2af-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ea2af-107">Return Type</span></span>    |<span data-ttu-id="ea2af-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea2af-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="ea2af-109">Get workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="ea2af-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="ea2af-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="ea2af-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="ea2af-111">Leia as propriedades e relacionamentos do objeto workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="ea2af-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="ea2af-112">Refresh</span><span class="sxs-lookup"><span data-stu-id="ea2af-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="ea2af-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ea2af-113">None</span></span>|<span data-ttu-id="ea2af-114">Atualiza a Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="ea2af-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="ea2af-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="ea2af-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="ea2af-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ea2af-116">None</span></span>|<span data-ttu-id="ea2af-p101">Atualização de todas as tabelas dentro de uma determinada planilha. Observe que esta ação está disponível somente na coleção de tabela dinâmica.</span><span class="sxs-lookup"><span data-stu-id="ea2af-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="ea2af-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ea2af-119">Properties</span></span>
| <span data-ttu-id="ea2af-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea2af-120">Property</span></span>     | <span data-ttu-id="ea2af-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea2af-121">Type</span></span>   |<span data-ttu-id="ea2af-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea2af-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea2af-123">id</span><span class="sxs-lookup"><span data-stu-id="ea2af-123">id</span></span>|<span data-ttu-id="ea2af-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ea2af-124">String</span></span>| <span data-ttu-id="ea2af-125">Id da Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="ea2af-125">Id of the PivotTable.</span></span>   <span data-ttu-id="ea2af-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea2af-126">Read-only.</span></span>|
|<span data-ttu-id="ea2af-127">nome</span><span class="sxs-lookup"><span data-stu-id="ea2af-127">name</span></span>|<span data-ttu-id="ea2af-128">String</span><span class="sxs-lookup"><span data-stu-id="ea2af-128">String</span></span>|<span data-ttu-id="ea2af-129">Nome da Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="ea2af-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="ea2af-130">Relações</span><span class="sxs-lookup"><span data-stu-id="ea2af-130">Relationships</span></span>
| <span data-ttu-id="ea2af-131">Relação</span><span class="sxs-lookup"><span data-stu-id="ea2af-131">Relationship</span></span> | <span data-ttu-id="ea2af-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea2af-132">Type</span></span>   |<span data-ttu-id="ea2af-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea2af-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ea2af-134">planilha</span><span class="sxs-lookup"><span data-stu-id="ea2af-134">worksheet</span></span>|[<span data-ttu-id="ea2af-135">worksheet</span><span class="sxs-lookup"><span data-stu-id="ea2af-135">worksheet</span></span>](worksheet.md)| <span data-ttu-id="ea2af-p103">A planilha que contém a Tabela Dinâmica atual. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ea2af-p103">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="ea2af-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea2af-138">JSON representation</span></span>
<span data-ttu-id="ea2af-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ea2af-139">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookPivotTable"
}-->

```json
{
  "id": "String (identifier)",
  "name": "String"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/workbookpivottable.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
