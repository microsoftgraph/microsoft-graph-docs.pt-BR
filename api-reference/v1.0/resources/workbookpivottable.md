---
title: tipo de recurso de tabela dinâmica
description: Representa uma Tabela Dinâmica do Excel.
author: lumine2008
ms.openlocfilehash: 68075aebeac9c0846e48739daf65e5bf97e4d6f5
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334108"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="85cef-103">tipo de recurso de tabela dinâmica</span><span class="sxs-lookup"><span data-stu-id="85cef-103">pivotTable resource type</span></span>

<span data-ttu-id="85cef-104">Representa uma Tabela Dinâmica do Excel.</span><span class="sxs-lookup"><span data-stu-id="85cef-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="85cef-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="85cef-105">Methods</span></span>

| <span data-ttu-id="85cef-106">Método</span><span class="sxs-lookup"><span data-stu-id="85cef-106">Method</span></span>           | <span data-ttu-id="85cef-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="85cef-107">Return Type</span></span>    |<span data-ttu-id="85cef-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="85cef-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="85cef-109">Get workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="85cef-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="85cef-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="85cef-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="85cef-111">Leia as propriedades e relacionamentos do objeto workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="85cef-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="85cef-112">Refresh</span><span class="sxs-lookup"><span data-stu-id="85cef-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="85cef-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="85cef-113">None</span></span>|<span data-ttu-id="85cef-114">Atualiza a Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="85cef-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="85cef-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="85cef-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="85cef-116">None</span><span class="sxs-lookup"><span data-stu-id="85cef-116">None</span></span>|<span data-ttu-id="85cef-p101">Atualização de todas as tabelas dentro de uma determinada planilha. Observe que esta ação está disponível somente na coleção de tabela dinâmica.</span><span class="sxs-lookup"><span data-stu-id="85cef-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="85cef-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="85cef-119">Properties</span></span>
| <span data-ttu-id="85cef-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="85cef-120">Property</span></span>     | <span data-ttu-id="85cef-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="85cef-121">Type</span></span>   |<span data-ttu-id="85cef-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="85cef-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85cef-123">id</span><span class="sxs-lookup"><span data-stu-id="85cef-123">id</span></span>|<span data-ttu-id="85cef-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="85cef-124">String</span></span>| <span data-ttu-id="85cef-p102">Id da Tabela Dinâmica.   Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="85cef-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="85cef-127">name</span><span class="sxs-lookup"><span data-stu-id="85cef-127">name</span></span>|<span data-ttu-id="85cef-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="85cef-128">String</span></span>|<span data-ttu-id="85cef-129">Nome da Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="85cef-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="85cef-130">Relações</span><span class="sxs-lookup"><span data-stu-id="85cef-130">Relationships</span></span>
| <span data-ttu-id="85cef-131">Relação</span><span class="sxs-lookup"><span data-stu-id="85cef-131">Relationship</span></span> | <span data-ttu-id="85cef-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="85cef-132">Type</span></span>   |<span data-ttu-id="85cef-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="85cef-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85cef-134">planilha</span><span class="sxs-lookup"><span data-stu-id="85cef-134">worksheet</span></span>|[<span data-ttu-id="85cef-135">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="85cef-135">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="85cef-p103">A planilha que contém a Tabela Dinâmica atual. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="85cef-p103">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="85cef-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="85cef-138">JSON representation</span></span>
<span data-ttu-id="85cef-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="85cef-139">Here is a JSON representation of the resource.</span></span>

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
