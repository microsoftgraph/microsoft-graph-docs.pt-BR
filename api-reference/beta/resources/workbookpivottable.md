---
title: tipo de recurso de tabela dinâmica
description: Representa uma Tabela Dinâmica do Excel.
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 91035b607d8c44f2d1515e9c004abd4c2235c0ec
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950855"
---
# <a name="pivottable-resource-type"></a><span data-ttu-id="95ff0-103">tipo de recurso de tabela dinâmica</span><span class="sxs-lookup"><span data-stu-id="95ff0-103">pivotTable resource type</span></span>

> <span data-ttu-id="95ff0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="95ff0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="95ff0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="95ff0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="95ff0-106">Representa uma Tabela Dinâmica do Excel.</span><span class="sxs-lookup"><span data-stu-id="95ff0-106">Represents an Excel PivotTable.</span></span>

## <a name="methods"></a><span data-ttu-id="95ff0-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="95ff0-107">Methods</span></span>

| <span data-ttu-id="95ff0-108">Método</span><span class="sxs-lookup"><span data-stu-id="95ff0-108">Method</span></span>           | <span data-ttu-id="95ff0-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="95ff0-109">Return Type</span></span>    |<span data-ttu-id="95ff0-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="95ff0-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="95ff0-111">Get workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="95ff0-111">Get workbookPivotTable</span></span>](../api/workbookpivottable-get.md) | [<span data-ttu-id="95ff0-112">workbookPivotTable</span><span class="sxs-lookup"><span data-stu-id="95ff0-112">workbookPivotTable</span></span>](workbookpivottable.md) |<span data-ttu-id="95ff0-113">Leia as propriedades e relacionamentos do objeto workbookPivotTable.</span><span class="sxs-lookup"><span data-stu-id="95ff0-113">Read properties and relationships of workbookPivotTable object.</span></span>|
|[<span data-ttu-id="95ff0-114">Refresh</span><span class="sxs-lookup"><span data-stu-id="95ff0-114">Refresh</span></span>](../api/workbookpivottable-refresh.md)|<span data-ttu-id="95ff0-115">Nenhum</span><span class="sxs-lookup"><span data-stu-id="95ff0-115">None</span></span>|<span data-ttu-id="95ff0-116">Atualiza a Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="95ff0-116">Refreshes the PivotTable.</span></span> |
|[<span data-ttu-id="95ff0-117">Refreshall</span><span class="sxs-lookup"><span data-stu-id="95ff0-117">Refreshall</span></span>](../api/workbookpivottable-refreshall.md)|<span data-ttu-id="95ff0-118">None</span><span class="sxs-lookup"><span data-stu-id="95ff0-118">None</span></span>|<span data-ttu-id="95ff0-p102">Atualização de todas as tabelas dentro de uma determinada planilha. Observe que esta ação está disponível somente na coleção de tabela dinâmica.</span><span class="sxs-lookup"><span data-stu-id="95ff0-p102">Refresh all tables within given worksheet. Note that this action is available only on the pivot table collection.</span></span>|

## <a name="properties"></a><span data-ttu-id="95ff0-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="95ff0-121">Properties</span></span>
| <span data-ttu-id="95ff0-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="95ff0-122">Property</span></span>     | <span data-ttu-id="95ff0-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="95ff0-123">Type</span></span>   |<span data-ttu-id="95ff0-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="95ff0-124">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95ff0-125">id</span><span class="sxs-lookup"><span data-stu-id="95ff0-125">id</span></span>|<span data-ttu-id="95ff0-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="95ff0-126">String</span></span>| <span data-ttu-id="95ff0-p103">Id da Tabela Dinâmica.   Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="95ff0-p103">Id of the PivotTable.   Read-only.</span></span>|
|<span data-ttu-id="95ff0-129">name</span><span class="sxs-lookup"><span data-stu-id="95ff0-129">name</span></span>|<span data-ttu-id="95ff0-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="95ff0-130">String</span></span>|<span data-ttu-id="95ff0-131">Nome da Tabela Dinâmica.</span><span class="sxs-lookup"><span data-stu-id="95ff0-131">Name of the PivotTable.</span></span>    |

## <a name="relationships"></a><span data-ttu-id="95ff0-132">Relações</span><span class="sxs-lookup"><span data-stu-id="95ff0-132">Relationships</span></span>
| <span data-ttu-id="95ff0-133">Relação</span><span class="sxs-lookup"><span data-stu-id="95ff0-133">Relationship</span></span> | <span data-ttu-id="95ff0-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="95ff0-134">Type</span></span>   |<span data-ttu-id="95ff0-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="95ff0-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95ff0-136">planilha</span><span class="sxs-lookup"><span data-stu-id="95ff0-136">worksheet</span></span>|[<span data-ttu-id="95ff0-137">worksheet</span><span class="sxs-lookup"><span data-stu-id="95ff0-137">worksheet</span></span>](worksheet.md)| <span data-ttu-id="95ff0-p104">A planilha que contém a Tabela Dinâmica atual. Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="95ff0-p104">The worksheet containing the current PivotTable. Read-only.</span></span>   |

## <a name="json-representation"></a><span data-ttu-id="95ff0-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="95ff0-140">JSON representation</span></span>
<span data-ttu-id="95ff0-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="95ff0-141">Here is a JSON representation of the resource.</span></span>

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
