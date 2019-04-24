---
title: tipo de recurso de tabela dinâmica
description: Representa uma Tabela Dinâmica do Excel.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 5f6360ce1eacc313f1bcc8a9f59b44b216a87b84
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456861"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="e31bb-103">tipo de recurso de tabela dinâmica</span><span class="sxs-lookup"><span data-stu-id="e31bb-103">pivotTable resource type</span></span>

<span data-ttu-id="e31bb-104">Representa uma Tabela Dinâmica do Excel.</span><span class="sxs-lookup"><span data-stu-id="e31bb-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="e31bb-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="e31bb-105">Methods</span></span>

| <span data-ttu-id="e31bb-106">Método</span><span class="sxs-lookup"><span data-stu-id="e31bb-106">Method</span></span>           | <span data-ttu-id="e31bb-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e31bb-107">Return Type</span></span>    |<span data-ttu-id="e31bb-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="e31bb-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e31bb-109">Get workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="e31bb-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="e31bb-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="e31bb-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="e31bb-111">Leia as propriedades e relacionamentos do objeto workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="e31bb-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="e31bb-112">Refresh</span><span class="sxs-lookup"><span data-stu-id="e31bb-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="e31bb-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e31bb-113">None</span></span>|<span data-ttu-id="e31bb-114">Atualiza a Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="e31bb-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="e31bb-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="e31bb-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="e31bb-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e31bb-116">None</span></span>|<span data-ttu-id="e31bb-p101">Atualização de todas as tabelas dentro de uma determinada planilha. Observe que esta ação está disponível somente na coleção de tabela dinâmica.</span><span class="sxs-lookup"><span data-stu-id="e31bb-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="e31bb-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e31bb-119">Properties</span></span>
| <span data-ttu-id="e31bb-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e31bb-120">Property</span></span>     | <span data-ttu-id="e31bb-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="e31bb-121">Type</span></span>   |<span data-ttu-id="e31bb-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="e31bb-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e31bb-123">id</span><span class="sxs-lookup"><span data-stu-id="e31bb-123">id</span></span>|<span data-ttu-id="e31bb-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e31bb-124">String</span></span>| <span data-ttu-id="e31bb-125">Id da Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="e31bb-125">Id of the PivotTable.</span></span>   <span data-ttu-id="e31bb-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e31bb-126">Read-only.</span></span>|
|<span data-ttu-id="e31bb-127">nome</span><span class="sxs-lookup"><span data-stu-id="e31bb-127">name</span></span>|<span data-ttu-id="e31bb-128">String</span><span class="sxs-lookup"><span data-stu-id="e31bb-128">String</span></span>|<span data-ttu-id="e31bb-129">Nome da Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="e31bb-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="e31bb-130">Relações</span><span class="sxs-lookup"><span data-stu-id="e31bb-130">Relationships</span></span>
| <span data-ttu-id="e31bb-131">Relação</span><span class="sxs-lookup"><span data-stu-id="e31bb-131">Relationship</span></span> | <span data-ttu-id="e31bb-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="e31bb-132">Type</span></span>   |<span data-ttu-id="e31bb-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="e31bb-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e31bb-134">planilha</span><span class="sxs-lookup"><span data-stu-id="e31bb-134">worksheet</span></span>|[<span data-ttu-id="e31bb-135">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="e31bb-135">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="e31bb-136">A planilha que contém a Tabela Dinâmica atual.</span><span class="sxs-lookup"><span data-stu-id="e31bb-136">The worksheet containing the current PivotTable.</span></span> <span data-ttu-id="e31bb-137">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e31bb-137">Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="e31bb-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e31bb-138">JSON representation</span></span>
<span data-ttu-id="e31bb-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e31bb-139">Here is a JSON representation of the resource.</span></span>

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
