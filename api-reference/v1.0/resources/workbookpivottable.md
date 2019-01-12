---
title: tipo de recurso de tabela dinâmica
description: Representa uma Tabela Dinâmica do Excel.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5f6360ce1eacc313f1bcc8a9f59b44b216a87b84
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27958737"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="16fba-103">tipo de recurso de tabela dinâmica</span><span class="sxs-lookup"><span data-stu-id="16fba-103">pivotTable resource type</span></span>

<span data-ttu-id="16fba-104">Representa uma Tabela Dinâmica do Excel.</span><span class="sxs-lookup"><span data-stu-id="16fba-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="16fba-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="16fba-105">Methods</span></span>

| <span data-ttu-id="16fba-106">Método</span><span class="sxs-lookup"><span data-stu-id="16fba-106">Method</span></span>           | <span data-ttu-id="16fba-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="16fba-107">Return Type</span></span>    |<span data-ttu-id="16fba-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="16fba-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="16fba-109">Get workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="16fba-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="16fba-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="16fba-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="16fba-111">Leia as propriedades e relacionamentos do objeto workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="16fba-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="16fba-112">Refresh</span><span class="sxs-lookup"><span data-stu-id="16fba-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="16fba-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="16fba-113">None</span></span>|<span data-ttu-id="16fba-114">Atualiza a Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="16fba-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="16fba-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="16fba-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="16fba-116">None</span><span class="sxs-lookup"><span data-stu-id="16fba-116">None</span></span>|<span data-ttu-id="16fba-p101">Atualização de todas as tabelas dentro de uma determinada planilha. Observe que esta ação está disponível somente na coleção de tabela dinâmica.</span><span class="sxs-lookup"><span data-stu-id="16fba-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="16fba-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="16fba-119">Properties</span></span>
| <span data-ttu-id="16fba-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="16fba-120">Property</span></span>     | <span data-ttu-id="16fba-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="16fba-121">Type</span></span>   |<span data-ttu-id="16fba-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="16fba-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16fba-123">id</span><span class="sxs-lookup"><span data-stu-id="16fba-123">id</span></span>|<span data-ttu-id="16fba-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16fba-124">String</span></span>| <span data-ttu-id="16fba-p102">Id da Tabela Dinâmica.   Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="16fba-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="16fba-127">name</span><span class="sxs-lookup"><span data-stu-id="16fba-127">name</span></span>|<span data-ttu-id="16fba-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="16fba-128">String</span></span>|<span data-ttu-id="16fba-129">Nome da Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="16fba-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="16fba-130">Relações</span><span class="sxs-lookup"><span data-stu-id="16fba-130">Relationships</span></span>
| <span data-ttu-id="16fba-131">Relação</span><span class="sxs-lookup"><span data-stu-id="16fba-131">Relationship</span></span> | <span data-ttu-id="16fba-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="16fba-132">Type</span></span>   |<span data-ttu-id="16fba-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="16fba-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16fba-134">planilha</span><span class="sxs-lookup"><span data-stu-id="16fba-134">worksheet</span></span>|[<span data-ttu-id="16fba-135">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="16fba-135">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="16fba-p103">A planilha que contém a Tabela Dinâmica atual. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="16fba-p103">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="16fba-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="16fba-138">JSON representation</span></span>
<span data-ttu-id="16fba-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="16fba-139">Here is a JSON representation of the resource.</span></span>

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
