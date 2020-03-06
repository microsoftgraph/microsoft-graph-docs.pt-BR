---
title: tipo de recurso de tabela dinâmica
description: Representa uma Tabela Dinâmica do Excel.
author: lumine2008
localization_priority: Normal
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: b3ec3c9237e246b2af10a867155bc7b6d360a67f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533380"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="6b8f8-103">tipo de recurso de tabela dinâmica</span><span class="sxs-lookup"><span data-stu-id="6b8f8-103">pivotTable resource type</span></span>

<span data-ttu-id="6b8f8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b8f8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6b8f8-105">Representa uma Tabela Dinâmica do Excel.</span><span class="sxs-lookup"><span data-stu-id="6b8f8-105">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="6b8f8-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="6b8f8-106">Methods</span></span>

| <span data-ttu-id="6b8f8-107">Método</span><span class="sxs-lookup"><span data-stu-id="6b8f8-107">Method</span></span>           | <span data-ttu-id="6b8f8-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6b8f8-108">Return Type</span></span>    |<span data-ttu-id="6b8f8-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b8f8-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6b8f8-110">Get workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="6b8f8-110">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="6b8f8-111">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="6b8f8-111">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="6b8f8-112">Leia as propriedades e relacionamentos do objeto workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="6b8f8-112">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="6b8f8-113">Refresh</span><span class="sxs-lookup"><span data-stu-id="6b8f8-113">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="6b8f8-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6b8f8-114">None</span></span>|<span data-ttu-id="6b8f8-115">Atualiza a Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="6b8f8-115">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="6b8f8-116">Refreshall</span><span class="sxs-lookup"><span data-stu-id="6b8f8-116">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="6b8f8-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6b8f8-117">None</span></span>|<span data-ttu-id="6b8f8-p101">Atualização de todas as tabelas dentro de uma determinada planilha. Observe que esta ação está disponível somente na coleção de tabela dinâmica.</span><span class="sxs-lookup"><span data-stu-id="6b8f8-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="6b8f8-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6b8f8-120">Properties</span></span>
| <span data-ttu-id="6b8f8-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b8f8-121">Property</span></span>     | <span data-ttu-id="6b8f8-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b8f8-122">Type</span></span>   |<span data-ttu-id="6b8f8-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b8f8-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b8f8-124">id</span><span class="sxs-lookup"><span data-stu-id="6b8f8-124">id</span></span>|<span data-ttu-id="6b8f8-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b8f8-125">String</span></span>| <span data-ttu-id="6b8f8-126">Id da Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="6b8f8-126">Id of the PivotTable.</span></span>   <span data-ttu-id="6b8f8-127">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6b8f8-127">Read-only.</span></span>|
|<span data-ttu-id="6b8f8-128">name</span><span class="sxs-lookup"><span data-stu-id="6b8f8-128">name</span></span>|<span data-ttu-id="6b8f8-129">String</span><span class="sxs-lookup"><span data-stu-id="6b8f8-129">String</span></span>|<span data-ttu-id="6b8f8-130">Nome da Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="6b8f8-130">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="6b8f8-131">Relacionamento</span><span class="sxs-lookup"><span data-stu-id="6b8f8-131">Relationships</span></span>
| <span data-ttu-id="6b8f8-132">Relação</span><span class="sxs-lookup"><span data-stu-id="6b8f8-132">Relationship</span></span> | <span data-ttu-id="6b8f8-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b8f8-133">Type</span></span>   |<span data-ttu-id="6b8f8-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b8f8-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b8f8-135">planilha</span><span class="sxs-lookup"><span data-stu-id="6b8f8-135">worksheet</span></span>|[<span data-ttu-id="6b8f8-136">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="6b8f8-136">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="6b8f8-137">A planilha que contém a Tabela Dinâmica atual.</span><span class="sxs-lookup"><span data-stu-id="6b8f8-137">The worksheet containing the current PivotTable.</span></span> <span data-ttu-id="6b8f8-138">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6b8f8-138">Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="6b8f8-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6b8f8-139">JSON representation</span></span>
<span data-ttu-id="6b8f8-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6b8f8-140">Here is a JSON representation of the resource.</span></span>

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
