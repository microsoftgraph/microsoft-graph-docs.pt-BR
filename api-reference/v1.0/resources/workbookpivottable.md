---
title: tipo de recurso de tabela dinâmica
description: Representa uma Tabela Dinâmica do Excel.
ms.openlocfilehash: b4ddd0c1bb9e4ee13aaf3d1b4472c4e750e3a755
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004094"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="82e31-103">tipo de recurso de tabela dinâmica</span><span class="sxs-lookup"><span data-stu-id="82e31-103">pivotTable resource type</span></span>

<span data-ttu-id="82e31-104">Representa uma Tabela Dinâmica do Excel.</span><span class="sxs-lookup"><span data-stu-id="82e31-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="82e31-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="82e31-105">Methods</span></span>

| <span data-ttu-id="82e31-106">Método</span><span class="sxs-lookup"><span data-stu-id="82e31-106">Method</span></span>           | <span data-ttu-id="82e31-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="82e31-107">Return Type</span></span>    |<span data-ttu-id="82e31-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="82e31-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="82e31-109">Get workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="82e31-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="82e31-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="82e31-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="82e31-111">Leia as propriedades e relacionamentos do objeto workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="82e31-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="82e31-112">Refresh</span><span class="sxs-lookup"><span data-stu-id="82e31-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="82e31-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="82e31-113">None</span></span>|<span data-ttu-id="82e31-114">Atualiza a Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="82e31-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="82e31-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="82e31-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="82e31-116">None</span><span class="sxs-lookup"><span data-stu-id="82e31-116">None</span></span>|<span data-ttu-id="82e31-p101">Atualização de todas as tabelas dentro de uma determinada planilha. Observe que esta ação está disponível somente na coleção de tabela dinâmica.</span><span class="sxs-lookup"><span data-stu-id="82e31-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="82e31-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="82e31-119">Properties</span></span>
| <span data-ttu-id="82e31-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="82e31-120">Property</span></span>     | <span data-ttu-id="82e31-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="82e31-121">Type</span></span>   |<span data-ttu-id="82e31-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="82e31-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82e31-123">id</span><span class="sxs-lookup"><span data-stu-id="82e31-123">id</span></span>|<span data-ttu-id="82e31-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="82e31-124">String</span></span>| <span data-ttu-id="82e31-p102">Id da Tabela Dinâmica.   Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="82e31-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="82e31-127">name</span><span class="sxs-lookup"><span data-stu-id="82e31-127">name</span></span>|<span data-ttu-id="82e31-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="82e31-128">String</span></span>|<span data-ttu-id="82e31-129">Nome da Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="82e31-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="82e31-130">Relações</span><span class="sxs-lookup"><span data-stu-id="82e31-130">Relationships</span></span>
| <span data-ttu-id="82e31-131">Relação</span><span class="sxs-lookup"><span data-stu-id="82e31-131">Relationship</span></span> | <span data-ttu-id="82e31-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="82e31-132">Type</span></span>   |<span data-ttu-id="82e31-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="82e31-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="82e31-134">planilha</span><span class="sxs-lookup"><span data-stu-id="82e31-134">worksheet</span></span>|[<span data-ttu-id="82e31-135">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="82e31-135">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="82e31-p103">A planilha que contém a Tabela Dinâmica atual. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="82e31-p103">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="82e31-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="82e31-138">JSON representation</span></span>
<span data-ttu-id="82e31-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="82e31-139">Here is a JSON representation of the resource.</span></span>

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
