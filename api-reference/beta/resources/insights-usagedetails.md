---
title: tipo de recurso usageDetails
description: Tipo complexo contendo propriedades de itens usados. Informações sobre quando o recurso foi acessado pela última vez (exibido) ou modificado (editado) pelo usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 553de0e8df9b3853024ffc35cc61bf6d727a2c9b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47986062"
---
# <a name="usagedetails-resource-type"></a><span data-ttu-id="b6bb4-104">tipo de recurso usageDetails</span><span class="sxs-lookup"><span data-stu-id="b6bb4-104">usageDetails resource type</span></span>

<span data-ttu-id="b6bb4-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6bb4-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b6bb4-106">Tipo complexo contendo propriedades de itens [usados](insights-used.md) .</span><span class="sxs-lookup"><span data-stu-id="b6bb4-106">Complex type containing properties of [Used](insights-used.md) items.</span></span> <span data-ttu-id="b6bb4-107">Informações sobre quando o recurso foi acessado pela última vez (exibido) ou modificado (editado) pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="b6bb4-107">Information on when the resource was last accessed (viewed) or modified (edited) by the user.</span></span>


## <a name="json-representation"></a><span data-ttu-id="b6bb4-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b6bb4-108">JSON representation</span></span>

<span data-ttu-id="b6bb4-109">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b6bb4-109">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.usageDetails"
}-->

```json
{
  "lastAccessedDateTime": "DateTimeOffset",
  "lastModifiedDateTime": "DateTimeOffset"
}
```

## <a name="properties"></a><span data-ttu-id="b6bb4-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b6bb4-110">Properties</span></span>

| <span data-ttu-id="b6bb4-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6bb4-111">Property</span></span>              | <span data-ttu-id="b6bb4-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6bb4-112">Type</span></span>          | <span data-ttu-id="b6bb4-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6bb4-113">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="b6bb4-114">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6bb4-114">lastAccessedDateTime</span></span>                  | <span data-ttu-id="b6bb4-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6bb4-115">DateTimeOffset</span></span>        | <span data-ttu-id="b6bb4-116">A data e a hora em que o recurso foi acessado pela última vez pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="b6bb4-116">The date and time the resource was last accessed by the user.</span></span> <span data-ttu-id="b6bb4-117">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b6bb4-117">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b6bb4-118">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="b6bb4-118">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="b6bb4-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b6bb4-119">Read-only.</span></span>                      |
| <span data-ttu-id="b6bb4-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b6bb4-120">lastModifiedDateTime</span></span>              | <span data-ttu-id="b6bb4-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b6bb4-121">DateTimeOffset</span></span>        | <span data-ttu-id="b6bb4-122">A data e a hora em que o recurso foi modificado pela última vez pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="b6bb4-122">The date and time the resource was last modified by the user.</span></span> <span data-ttu-id="b6bb4-123">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b6bb4-123">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b6bb4-124">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="b6bb4-124">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="b6bb4-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b6bb4-125">Read-only.</span></span>       |


