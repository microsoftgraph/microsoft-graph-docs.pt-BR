---
title: tipo de recurso workbookApplication
description: Representa o aplicativo Excel que gerencia a pasta de trabalho.
localization_priority: Normal
author: grangeryy
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: d4b2833910d22696ee95ed707469f6da2068453c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446720"
---
# <a name="workbookapplication-resource-type"></a><span data-ttu-id="850d0-103">tipo de recurso workbookApplication</span><span class="sxs-lookup"><span data-stu-id="850d0-103">workbookApplication resource type</span></span>

<span data-ttu-id="850d0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="850d0-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="850d0-105">Representa o aplicativo Excel que gerencia a pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="850d0-105">Represents the Excel application that manages the workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="850d0-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="850d0-106">Methods</span></span>

| <span data-ttu-id="850d0-107">Método</span><span class="sxs-lookup"><span data-stu-id="850d0-107">Method</span></span>           | <span data-ttu-id="850d0-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="850d0-108">Return Type</span></span>    |<span data-ttu-id="850d0-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="850d0-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="850d0-110">Obter workbookApplication</span><span class="sxs-lookup"><span data-stu-id="850d0-110">Get workbookApplication</span></span>](../api/workbookapplication-get.md) | [<span data-ttu-id="850d0-111">workbookApplication</span><span class="sxs-lookup"><span data-stu-id="850d0-111">workbookApplication</span></span>](workbookapplication.md) |<span data-ttu-id="850d0-112">Leia as propriedades e os relacionamentos do objeto workbookApplication.</span><span class="sxs-lookup"><span data-stu-id="850d0-112">Read properties and relationships of workbookApplication object.</span></span>|
|[<span data-ttu-id="850d0-113">Calculate</span><span class="sxs-lookup"><span data-stu-id="850d0-113">Calculate</span></span>](../api/workbookapplication-calculate.md)|<span data-ttu-id="850d0-114">Nenhum</span><span class="sxs-lookup"><span data-stu-id="850d0-114">None</span></span>|<span data-ttu-id="850d0-115">Recalcula todas as pastas de trabalho abertas no Excel no momento.</span><span class="sxs-lookup"><span data-stu-id="850d0-115">Recalculate all currently opened workbooks in Excel.</span></span>|

## <a name="properties"></a><span data-ttu-id="850d0-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="850d0-116">Properties</span></span>
| <span data-ttu-id="850d0-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="850d0-117">Property</span></span>     | <span data-ttu-id="850d0-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="850d0-118">Type</span></span>   |<span data-ttu-id="850d0-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="850d0-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="850d0-120">cálculomode</span><span class="sxs-lookup"><span data-stu-id="850d0-120">calculationMode</span></span>|<span data-ttu-id="850d0-121">string</span><span class="sxs-lookup"><span data-stu-id="850d0-121">string</span></span>|<span data-ttu-id="850d0-122">Retorna o modo de cálculo usado na pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="850d0-122">Returns the calculation mode used in the workbook.</span></span> <span data-ttu-id="850d0-123">Os valores possíveis são: `Automatic`, `AutomaticExceptTables`, `Manual`.</span><span class="sxs-lookup"><span data-stu-id="850d0-123">Possible values are: `Automatic`, `AutomaticExceptTables`, `Manual`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="850d0-124">Relações</span><span class="sxs-lookup"><span data-stu-id="850d0-124">Relationships</span></span>
<span data-ttu-id="850d0-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="850d0-125">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="850d0-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="850d0-126">JSON representation</span></span>

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
