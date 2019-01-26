---
title: tipo de recurso de tabela dinâmica
description: Representa uma Tabela Dinâmica do Excel.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 774c407022d700bc5856dc780eff3a6dafa6bc4e
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577456"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="6ff78-103">tipo de recurso de tabela dinâmica</span><span class="sxs-lookup"><span data-stu-id="6ff78-103">pivotTable resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ff78-104">Representa uma Tabela Dinâmica do Excel.</span><span class="sxs-lookup"><span data-stu-id="6ff78-104">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="6ff78-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="6ff78-105">Methods</span></span>

| <span data-ttu-id="6ff78-106">Método</span><span class="sxs-lookup"><span data-stu-id="6ff78-106">Method</span></span>           | <span data-ttu-id="6ff78-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6ff78-107">Return Type</span></span>    |<span data-ttu-id="6ff78-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ff78-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6ff78-109">Get workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="6ff78-109">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="6ff78-110">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="6ff78-110">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="6ff78-111">Leia as propriedades e relacionamentos do objeto workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="6ff78-111">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="6ff78-112">Refresh</span><span class="sxs-lookup"><span data-stu-id="6ff78-112">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="6ff78-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6ff78-113">None</span></span>|<span data-ttu-id="6ff78-114">Atualiza a Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="6ff78-114">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="6ff78-115">Refreshall</span><span class="sxs-lookup"><span data-stu-id="6ff78-115">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="6ff78-116">None</span><span class="sxs-lookup"><span data-stu-id="6ff78-116">None</span></span>|<span data-ttu-id="6ff78-p101">Atualização de todas as tabelas dentro de uma determinada planilha. Observe que esta ação está disponível somente na coleção de tabela dinâmica.</span><span class="sxs-lookup"><span data-stu-id="6ff78-p101">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="6ff78-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6ff78-119">Properties</span></span>
| <span data-ttu-id="6ff78-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6ff78-120">Property</span></span>     | <span data-ttu-id="6ff78-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ff78-121">Type</span></span>   |<span data-ttu-id="6ff78-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ff78-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ff78-123">id</span><span class="sxs-lookup"><span data-stu-id="6ff78-123">id</span></span>|<span data-ttu-id="6ff78-124">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6ff78-124">String</span></span>| <span data-ttu-id="6ff78-p102">Id da Tabela Dinâmica.   Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6ff78-p102">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="6ff78-127">name</span><span class="sxs-lookup"><span data-stu-id="6ff78-127">name</span></span>|<span data-ttu-id="6ff78-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6ff78-128">String</span></span>|<span data-ttu-id="6ff78-129">Nome da Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="6ff78-129">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="6ff78-130">Relações</span><span class="sxs-lookup"><span data-stu-id="6ff78-130">Relationships</span></span>
| <span data-ttu-id="6ff78-131">Relação</span><span class="sxs-lookup"><span data-stu-id="6ff78-131">Relationship</span></span> | <span data-ttu-id="6ff78-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ff78-132">Type</span></span>   |<span data-ttu-id="6ff78-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ff78-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ff78-134">planilha</span><span class="sxs-lookup"><span data-stu-id="6ff78-134">worksheet</span></span>|[<span data-ttu-id="6ff78-135">WorkbookWorksheet</span><span class="sxs-lookup"><span data-stu-id="6ff78-135">WorkbookWorksheet</span></span>](worksheet.md)| <span data-ttu-id="6ff78-p103">A planilha que contém a Tabela Dinâmica atual. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6ff78-p103">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="6ff78-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6ff78-138">JSON representation</span></span>
<span data-ttu-id="6ff78-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6ff78-139">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/workbookpivottable.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
