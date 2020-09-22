---
title: tipo de recurso workbookPivotTable
description: Representa uma Tabela Dinâmica do Excel.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 98db064c101d60c9db25eb0a9515da74e25e96ad
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023814"
---
# <a name="workbookpivottable-resource-type"></a><span data-ttu-id="9ea1b-103">tipo de recurso workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="9ea1b-103">workbookPivotTable resource type</span></span>

<span data-ttu-id="9ea1b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ea1b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ea1b-105">Representa uma Tabela Dinâmica do Excel.</span><span class="sxs-lookup"><span data-stu-id="9ea1b-105">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="9ea1b-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="9ea1b-106">Methods</span></span>

| <span data-ttu-id="9ea1b-107">Método</span><span class="sxs-lookup"><span data-stu-id="9ea1b-107">Method</span></span>           | <span data-ttu-id="9ea1b-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9ea1b-108">Return Type</span></span>    |<span data-ttu-id="9ea1b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ea1b-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9ea1b-110">Get workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="9ea1b-110">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="9ea1b-111">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="9ea1b-111">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="9ea1b-112">Leia as propriedades e relacionamentos do objeto workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="9ea1b-112">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="9ea1b-113">Refresh</span><span class="sxs-lookup"><span data-stu-id="9ea1b-113">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="9ea1b-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9ea1b-114">None</span></span>|<span data-ttu-id="9ea1b-115">Atualiza a Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="9ea1b-115">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="9ea1b-116">Refreshall</span><span class="sxs-lookup"><span data-stu-id="9ea1b-116">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="9ea1b-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9ea1b-117">None</span></span>|<span data-ttu-id="9ea1b-p101">Atualização de todas as tabelas dentro de uma determinada planilha. Observe que esta ação está disponível somente na coleção de tabela dinâmica.</span><span class="sxs-lookup"><span data-stu-id="9ea1b-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="9ea1b-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9ea1b-120">Properties</span></span>
| <span data-ttu-id="9ea1b-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9ea1b-121">Property</span></span>     | <span data-ttu-id="9ea1b-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ea1b-122">Type</span></span>   |<span data-ttu-id="9ea1b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ea1b-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ea1b-124">id</span><span class="sxs-lookup"><span data-stu-id="9ea1b-124">id</span></span>|<span data-ttu-id="9ea1b-125">String</span><span class="sxs-lookup"><span data-stu-id="9ea1b-125">String</span></span>| <span data-ttu-id="9ea1b-126">Id da Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="9ea1b-126">Id of the PivotTable.</span></span>   <span data-ttu-id="9ea1b-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9ea1b-127">Read-only.</span></span>|
|<span data-ttu-id="9ea1b-128">name</span><span class="sxs-lookup"><span data-stu-id="9ea1b-128">name</span></span>|<span data-ttu-id="9ea1b-129">String</span><span class="sxs-lookup"><span data-stu-id="9ea1b-129">String</span></span>|<span data-ttu-id="9ea1b-130">Nome da Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="9ea1b-130">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="9ea1b-131">Relações</span><span class="sxs-lookup"><span data-stu-id="9ea1b-131">Relationships</span></span>
| <span data-ttu-id="9ea1b-132">Relação</span><span class="sxs-lookup"><span data-stu-id="9ea1b-132">Relationship</span></span> | <span data-ttu-id="9ea1b-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="9ea1b-133">Type</span></span>   |<span data-ttu-id="9ea1b-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="9ea1b-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9ea1b-135">planilha</span><span class="sxs-lookup"><span data-stu-id="9ea1b-135">worksheet</span></span>|[<span data-ttu-id="9ea1b-136">workbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="9ea1b-136">workbookWorksheet</span></span>](workbookworksheet.md)| <span data-ttu-id="9ea1b-137">A planilha que contém a Tabela Dinâmica atual.</span><span class="sxs-lookup"><span data-stu-id="9ea1b-137">The worksheet containing the current PivotTable.</span></span> <span data-ttu-id="9ea1b-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9ea1b-138">Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="9ea1b-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9ea1b-139">JSON representation</span></span>
<span data-ttu-id="9ea1b-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9ea1b-140">Here is a JSON representation of the resource.</span></span>

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


