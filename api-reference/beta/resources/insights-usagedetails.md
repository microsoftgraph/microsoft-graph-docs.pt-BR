---
title: tipo de recurso usageDetails
description: Tipo complexo contendo propriedades de itens usados. Informações sobre quando o recurso foi acessado pela última vez (exibido) e modificado (editado) pelo usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 550a71fa087870f708df2587454d9ebc05bbec1d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42495519"
---
# <a name="usagedetails-resource-type"></a><span data-ttu-id="2128f-104">tipo de recurso usageDetails</span><span class="sxs-lookup"><span data-stu-id="2128f-104">usageDetails resource type</span></span>

<span data-ttu-id="2128f-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2128f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2128f-106">Tipo complexo contendo propriedades de itens [usados](insights-used.md) .</span><span class="sxs-lookup"><span data-stu-id="2128f-106">Complex type containing properties of [used](insights-used.md) items.</span></span> <span data-ttu-id="2128f-107">Informações sobre quando o recurso foi acessado pela última vez (exibido) e modificado (editado) pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="2128f-107">Information on when the resource was last accessed (viewed) and modified (edited) by the user.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2128f-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2128f-108">JSON representation</span></span>

<span data-ttu-id="2128f-109">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="2128f-109">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="2128f-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2128f-110">Properties</span></span>

| <span data-ttu-id="2128f-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2128f-111">Property</span></span>              | <span data-ttu-id="2128f-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="2128f-112">Type</span></span>          | <span data-ttu-id="2128f-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="2128f-113">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="2128f-114">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="2128f-114">lastAccessedDateTime</span></span>                  | <span data-ttu-id="2128f-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2128f-115">DateTimeOffset</span></span>        | <span data-ttu-id="2128f-116">A data e a hora em que o recurso foi acessado pela última vez pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="2128f-116">The date and time the resource was last accessed by the user.</span></span> <span data-ttu-id="2128f-117">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="2128f-117">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2128f-118">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="2128f-118">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="2128f-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2128f-119">Read-only.</span></span>                      |
| <span data-ttu-id="2128f-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2128f-120">lastModifiedDateTime</span></span>              | <span data-ttu-id="2128f-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2128f-121">DateTimeOffset</span></span>        | <span data-ttu-id="2128f-122">A data e a hora em que o recurso foi modificado pela última vez pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="2128f-122">The date and time the resource was last modified by the user.</span></span> <span data-ttu-id="2128f-123">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="2128f-123">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2128f-124">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="2128f-124">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="2128f-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="2128f-125">Read-only.</span></span>       |
