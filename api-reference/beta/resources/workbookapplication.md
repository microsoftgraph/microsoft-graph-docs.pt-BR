---
title: tipo de recurso workbookApplication
description: Representa o workbookApplication do Excel que gerencia a pasta de trabalho.
localization_priority: Normal
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 3db8c640ebb2fd36a0902563c28a3ec51bfa99d8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33348496"
---
# <a name="workbookapplication-resource-type"></a><span data-ttu-id="6ce27-103">tipo de recurso workbookApplication</span><span class="sxs-lookup"><span data-stu-id="6ce27-103">workbookApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ce27-104">Representa o aplicativo Excel que gerencia a pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6ce27-104">Represents the Excel application that manages the workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="6ce27-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="6ce27-105">Methods</span></span>

| <span data-ttu-id="6ce27-106">Método</span><span class="sxs-lookup"><span data-stu-id="6ce27-106">Method</span></span>           | <span data-ttu-id="6ce27-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6ce27-107">Return Type</span></span>    |<span data-ttu-id="6ce27-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ce27-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="6ce27-109">Obter workbookApplication</span><span class="sxs-lookup"><span data-stu-id="6ce27-109">Get workbookApplication</span></span>](../api/workbookapplication-get.md) | [<span data-ttu-id="6ce27-110">workbookApplication</span><span class="sxs-lookup"><span data-stu-id="6ce27-110">workbookApplication</span></span>](workbookapplication.md) |<span data-ttu-id="6ce27-111">Leia as propriedades e os relacionamentos do objeto workbookApplication.</span><span class="sxs-lookup"><span data-stu-id="6ce27-111">Read properties and relationships of workbookApplication object.</span></span>|
|[<span data-ttu-id="6ce27-112">Calculate</span><span class="sxs-lookup"><span data-stu-id="6ce27-112">Calculate</span></span>](../api/workbookapplication-calculate.md)|<span data-ttu-id="6ce27-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6ce27-113">None</span></span>|<span data-ttu-id="6ce27-114">Recalcula todas as pastas de trabalho abertas no Excel no momento.</span><span class="sxs-lookup"><span data-stu-id="6ce27-114">Recalculate all currently opened workbooks in Excel.</span></span>|

## <a name="properties"></a><span data-ttu-id="6ce27-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6ce27-115">Properties</span></span>
| <span data-ttu-id="6ce27-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6ce27-116">Property</span></span>     | <span data-ttu-id="6ce27-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ce27-117">Type</span></span>   |<span data-ttu-id="6ce27-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ce27-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6ce27-119">cálculomode</span><span class="sxs-lookup"><span data-stu-id="6ce27-119">calculationMode</span></span>|<span data-ttu-id="6ce27-120">string</span><span class="sxs-lookup"><span data-stu-id="6ce27-120">string</span></span>|<span data-ttu-id="6ce27-121">Retorna o modo de cálculo usado na pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="6ce27-121">Returns the calculation mode used in the workbook.</span></span> <span data-ttu-id="6ce27-122">Os valores possíveis são: `Automatic`, `AutomaticExceptTables`, `Manual`.</span><span class="sxs-lookup"><span data-stu-id="6ce27-122">Possible values are: `Automatic`, `AutomaticExceptTables`, `Manual`.</span></span> <span data-ttu-id="6ce27-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6ce27-123">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6ce27-124">Relações</span><span class="sxs-lookup"><span data-stu-id="6ce27-124">Relationships</span></span>
<span data-ttu-id="6ce27-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6ce27-125">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6ce27-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6ce27-126">JSON representation</span></span>

<span data-ttu-id="6ce27-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6ce27-127">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.workbookApplication"
}-->

```json
{
  "calculationMode": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "workbookApplication resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
