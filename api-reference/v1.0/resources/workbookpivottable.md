---
title: tipo de recurso de tabela dinâmica
description: Representa uma Tabela Dinâmica do Excel.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: fb67920598d883a126c18cdf8acdfb1b38d9014a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48015131"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="e684d-103">tipo de recurso de tabela dinâmica</span><span class="sxs-lookup"><span data-stu-id="e684d-103">pivotTable resource type</span></span>

<span data-ttu-id="e684d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e684d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e684d-105">Representa uma Tabela Dinâmica do Excel.</span><span class="sxs-lookup"><span data-stu-id="e684d-105">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="e684d-106">Methods</span><span class="sxs-lookup"><span data-stu-id="e684d-106">Methods</span></span>

| <span data-ttu-id="e684d-107">Método</span><span class="sxs-lookup"><span data-stu-id="e684d-107">Method</span></span>           | <span data-ttu-id="e684d-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e684d-108">Return Type</span></span>    |<span data-ttu-id="e684d-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e684d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e684d-110">Get workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="e684d-110">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="e684d-111">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="e684d-111">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="e684d-112">Leia as propriedades e relacionamentos do objeto workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="e684d-112">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="e684d-113">Refresh</span><span class="sxs-lookup"><span data-stu-id="e684d-113">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="e684d-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e684d-114">None</span></span>|<span data-ttu-id="e684d-115">Atualiza a Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="e684d-115">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="e684d-116">Refreshall</span><span class="sxs-lookup"><span data-stu-id="e684d-116">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="e684d-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e684d-117">None</span></span>|<span data-ttu-id="e684d-p101">Atualização de todas as tabelas dentro de uma determinada planilha. Observe que esta ação está disponível somente na coleção de tabela dinâmica.</span><span class="sxs-lookup"><span data-stu-id="e684d-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="e684d-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e684d-120">Properties</span></span>
| <span data-ttu-id="e684d-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e684d-121">Property</span></span>     | <span data-ttu-id="e684d-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="e684d-122">Type</span></span>   |<span data-ttu-id="e684d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e684d-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e684d-124">id</span><span class="sxs-lookup"><span data-stu-id="e684d-124">id</span></span>|<span data-ttu-id="e684d-125">String</span><span class="sxs-lookup"><span data-stu-id="e684d-125">String</span></span>| <span data-ttu-id="e684d-126">Id da Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="e684d-126">Id of the PivotTable.</span></span>   <span data-ttu-id="e684d-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e684d-127">Read-only.</span></span>|
|<span data-ttu-id="e684d-128">name</span><span class="sxs-lookup"><span data-stu-id="e684d-128">name</span></span>|<span data-ttu-id="e684d-129">String</span><span class="sxs-lookup"><span data-stu-id="e684d-129">String</span></span>|<span data-ttu-id="e684d-130">Nome da Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="e684d-130">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="e684d-131">Relações</span><span class="sxs-lookup"><span data-stu-id="e684d-131">Relationships</span></span>
| <span data-ttu-id="e684d-132">Relação</span><span class="sxs-lookup"><span data-stu-id="e684d-132">Relationship</span></span> | <span data-ttu-id="e684d-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="e684d-133">Type</span></span>   |<span data-ttu-id="e684d-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="e684d-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e684d-135">planilha</span><span class="sxs-lookup"><span data-stu-id="e684d-135">worksheet</span></span>|[<span data-ttu-id="e684d-136">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="e684d-136">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="e684d-137">A planilha que contém a Tabela Dinâmica atual.</span><span class="sxs-lookup"><span data-stu-id="e684d-137">The worksheet containing the current PivotTable.</span></span> <span data-ttu-id="e684d-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e684d-138">Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="e684d-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e684d-139">JSON representation</span></span>
<span data-ttu-id="e684d-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e684d-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
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

