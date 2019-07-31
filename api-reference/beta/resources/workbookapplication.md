---
title: tipo de recurso workbookApplication
description: Representa o workbookApplication do Excel que gerencia a pasta de trabalho.
localization_priority: Normal
author: lumine2008
ms.prod: excel
doc_type: resourcePageType
ms.openlocfilehash: 71c7c92e623fc2a9c05b9e1e8448f329615c51e3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964106"
---
# <a name="workbookapplication-resource-type"></a><span data-ttu-id="55227-103">tipo de recurso workbookApplication</span><span class="sxs-lookup"><span data-stu-id="55227-103">workbookApplication resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55227-104">Representa o aplicativo Excel que gerencia a pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="55227-104">Represents the Excel application that manages the workbook.</span></span>


## <a name="methods"></a><span data-ttu-id="55227-105">Métodos</span><span class="sxs-lookup"><span data-stu-id="55227-105">Methods</span></span>

| <span data-ttu-id="55227-106">Método</span><span class="sxs-lookup"><span data-stu-id="55227-106">Method</span></span>           | <span data-ttu-id="55227-107">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="55227-107">Return Type</span></span>    |<span data-ttu-id="55227-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="55227-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="55227-109">Obter workbookApplication</span><span class="sxs-lookup"><span data-stu-id="55227-109">Get workbookApplication</span></span>](../api/workbookapplication-get.md) | [<span data-ttu-id="55227-110">workbookApplication</span><span class="sxs-lookup"><span data-stu-id="55227-110">workbookApplication</span></span>](workbookapplication.md) |<span data-ttu-id="55227-111">Leia as propriedades e os relacionamentos do objeto workbookApplication.</span><span class="sxs-lookup"><span data-stu-id="55227-111">Read properties and relationships of workbookApplication object.</span></span>|
|[<span data-ttu-id="55227-112">Calculate</span><span class="sxs-lookup"><span data-stu-id="55227-112">Calculate</span></span>](../api/workbookapplication-calculate.md)|<span data-ttu-id="55227-113">Nenhum</span><span class="sxs-lookup"><span data-stu-id="55227-113">None</span></span>|<span data-ttu-id="55227-114">Recalcula todas as pastas de trabalho abertas no Excel no momento.</span><span class="sxs-lookup"><span data-stu-id="55227-114">Recalculate all currently opened workbooks in Excel.</span></span>|

## <a name="properties"></a><span data-ttu-id="55227-115">Propriedades</span><span class="sxs-lookup"><span data-stu-id="55227-115">Properties</span></span>
| <span data-ttu-id="55227-116">Propriedade</span><span class="sxs-lookup"><span data-stu-id="55227-116">Property</span></span>     | <span data-ttu-id="55227-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="55227-117">Type</span></span>   |<span data-ttu-id="55227-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="55227-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55227-119">cálculomode</span><span class="sxs-lookup"><span data-stu-id="55227-119">calculationMode</span></span>|<span data-ttu-id="55227-120">string</span><span class="sxs-lookup"><span data-stu-id="55227-120">string</span></span>|<span data-ttu-id="55227-121">Retorna o modo de cálculo usado na pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="55227-121">Returns the calculation mode used in the workbook.</span></span> <span data-ttu-id="55227-122">Os valores possíveis são: `Automatic`, `AutomaticExceptTables`, `Manual`.</span><span class="sxs-lookup"><span data-stu-id="55227-122">Possible values are: `Automatic`, `AutomaticExceptTables`, `Manual`.</span></span> <span data-ttu-id="55227-123">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="55227-123">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55227-124">Relações</span><span class="sxs-lookup"><span data-stu-id="55227-124">Relationships</span></span>
<span data-ttu-id="55227-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="55227-125">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="55227-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="55227-126">JSON representation</span></span>

<span data-ttu-id="55227-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="55227-127">Here is a JSON representation of the resource.</span></span>

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
