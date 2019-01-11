---
title: tipo de recurso de tabela dinâmica
description: Representa uma Tabela Dinâmica do Excel.
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: d500d4bc88608b032262cfae505385bf7ed3f072
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889205"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="6ccab-103">tipo de recurso de tabela dinâmica</span><span class="sxs-lookup"><span data-stu-id="6ccab-103">pivotTable resource type</span></span>

<span data-ttu-id="6ccab-104">Representa uma Tabela Dinâmica do Excel.</span><span class="sxs-lookup"><span data-stu-id="6ccab-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="6ccab-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="6ccab-105">Methods</span></span>

| <span data-ttu-id="6ccab-106">Método</span><span class="sxs-lookup"><span data-stu-id="6ccab-106">Method</span></span>           | <span data-ttu-id="6ccab-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6ccab-107">Return Type</span></span>    |<span data-ttu-id="6ccab-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ccab-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6ccab-109">Get workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="6ccab-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="6ccab-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="6ccab-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="6ccab-111">Leia as propriedades e relacionamentos do objeto workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="6ccab-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="6ccab-112">Refresh</span><span class="sxs-lookup"><span data-stu-id="6ccab-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="6ccab-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6ccab-113">None</span></span>|<span data-ttu-id="6ccab-114">Atualiza a Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="6ccab-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="6ccab-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="6ccab-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="6ccab-116">None</span><span class="sxs-lookup"><span data-stu-id="6ccab-116">None</span></span>|<span data-ttu-id="6ccab-p101">Atualização de todas as tabelas dentro de uma determinada planilha. Observe que esta ação está disponível somente na coleção de tabela dinâmica.</span><span class="sxs-lookup"><span data-stu-id="6ccab-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="6ccab-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6ccab-119">Properties</span></span>
| <span data-ttu-id="6ccab-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6ccab-120">Property</span></span>     | <span data-ttu-id="6ccab-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ccab-121">Type</span></span>   |<span data-ttu-id="6ccab-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ccab-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ccab-123">id</span><span class="sxs-lookup"><span data-stu-id="6ccab-123">id</span></span>|<span data-ttu-id="6ccab-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6ccab-124">String</span></span>| <span data-ttu-id="6ccab-p102">Id da Tabela Dinâmica.   Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6ccab-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="6ccab-127">name</span><span class="sxs-lookup"><span data-stu-id="6ccab-127">name</span></span>|<span data-ttu-id="6ccab-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6ccab-128">String</span></span>|<span data-ttu-id="6ccab-129">Nome da Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="6ccab-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="6ccab-130">Relações</span><span class="sxs-lookup"><span data-stu-id="6ccab-130">Relationships</span></span>
| <span data-ttu-id="6ccab-131">Relação</span><span class="sxs-lookup"><span data-stu-id="6ccab-131">Relationship</span></span> | <span data-ttu-id="6ccab-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ccab-132">Type</span></span>   |<span data-ttu-id="6ccab-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ccab-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ccab-134">planilha</span><span class="sxs-lookup"><span data-stu-id="6ccab-134">worksheet</span></span>|[<span data-ttu-id="6ccab-135">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="6ccab-135">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="6ccab-p103">A planilha que contém a Tabela Dinâmica atual. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6ccab-p103">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="6ccab-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6ccab-138">JSON representation</span></span>
<span data-ttu-id="6ccab-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6ccab-139">Here is a JSON representation of the resource.</span></span>

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
