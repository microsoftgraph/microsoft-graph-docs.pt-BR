---
title: tipo de recurso workbookApplication
description: Representa o workbookApplication do Excel que gerencia a pasta de trabalho.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 04b2d4ab31651fe34affe42ef4811c3802762581
ms.sourcegitcommit: 2f3e7325b5bc1f0cdc12a8acdf34d31cea3b8bdb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/07/2019
ms.locfileid: "38023195"
---
# <a name="workbookapplication-resource-type"></a><span data-ttu-id="7f146-103">tipo de recurso workbookApplication</span><span class="sxs-lookup"><span data-stu-id="7f146-103">workbookApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f146-104">Representa o aplicativo Excel que gerencia a pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="7f146-104">Represents the Excel application that manages the workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="7f146-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="7f146-105">Methods</span></span>

| <span data-ttu-id="7f146-106">Método</span><span class="sxs-lookup"><span data-stu-id="7f146-106">Method</span></span>           | <span data-ttu-id="7f146-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="7f146-107">Return Type</span></span>    |<span data-ttu-id="7f146-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f146-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7f146-109">Obter workbookApplication</span><span class="sxs-lookup"><span data-stu-id="7f146-109">Get workbookApplication</span></span>](../api/workbookapplication-get.md) | [<span data-ttu-id="7f146-110">workbookApplication</span><span class="sxs-lookup"><span data-stu-id="7f146-110">workbookApplication</span></span>](workbookapplication.md) |<span data-ttu-id="7f146-111">Leia as propriedades e os relacionamentos do objeto workbookApplication.</span><span class="sxs-lookup"><span data-stu-id="7f146-111">Read properties and relationships of workbookApplication object.</span></span>|
|[<span data-ttu-id="7f146-112">Calculate</span><span class="sxs-lookup"><span data-stu-id="7f146-112">Calculate</span></span>](../api/workbookapplication-calculate.md)|<span data-ttu-id="7f146-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7f146-113">None</span></span>|<span data-ttu-id="7f146-114">Recalcula todas as pastas de trabalho abertas no Excel no momento.</span><span class="sxs-lookup"><span data-stu-id="7f146-114">Recalculate all currently opened workbooks in Excel.</span></span>|

## <a name="properties"></a><span data-ttu-id="7f146-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7f146-115">Properties</span></span>
| <span data-ttu-id="7f146-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7f146-116">Property</span></span>     | <span data-ttu-id="7f146-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="7f146-117">Type</span></span>   |<span data-ttu-id="7f146-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="7f146-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7f146-119">cálculomode</span><span class="sxs-lookup"><span data-stu-id="7f146-119">calculationMode</span></span>|<span data-ttu-id="7f146-120">string</span><span class="sxs-lookup"><span data-stu-id="7f146-120">string</span></span>|<span data-ttu-id="7f146-121">Retorna o modo de cálculo usado na pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="7f146-121">Returns the calculation mode used in the workbook.</span></span> <span data-ttu-id="7f146-122">Os valores possíveis são: `Automatic`, `AutomaticExceptTables`, `Manual`.</span><span class="sxs-lookup"><span data-stu-id="7f146-122">Possible values are: `Automatic`, `AutomaticExceptTables`, `Manual`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7f146-123">Relações</span><span class="sxs-lookup"><span data-stu-id="7f146-123">Relationships</span></span>
<span data-ttu-id="7f146-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7f146-124">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="7f146-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7f146-125">JSON representation</span></span>


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
