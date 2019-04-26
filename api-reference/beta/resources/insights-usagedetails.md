---
title: tipo de recurso usageDetails
description: Tipo complexo contendo propriedades de itens usados. Informações sobre quando o recurso foi acessado pela última vez (exibido) e modificado (editado) pelo usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: d8a8893f2c5fcb21e2e578eefa4cf5733782db07
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333530"
---
# <a name="usagedetails-resource-type"></a><span data-ttu-id="9fc82-104">tipo de recurso usageDetails</span><span class="sxs-lookup"><span data-stu-id="9fc82-104">usageDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9fc82-105">Tipo complexo contendo propriedades de itens [usados](insights-used.md) .</span><span class="sxs-lookup"><span data-stu-id="9fc82-105">Complex type containing properties of [Used](insights-used.md) items.</span></span> <span data-ttu-id="9fc82-106">Informações sobre quando o recurso foi acessado pela última vez (exibido) e modificado (editado) pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="9fc82-106">Information on when the resource was last accessed (viewed) and modified (edited) by the user.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9fc82-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9fc82-107">JSON representation</span></span>

<span data-ttu-id="9fc82-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="9fc82-108">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="9fc82-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9fc82-109">Properties</span></span>

| <span data-ttu-id="9fc82-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9fc82-110">Property</span></span>              | <span data-ttu-id="9fc82-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="9fc82-111">Type</span></span>          | <span data-ttu-id="9fc82-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="9fc82-112">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="9fc82-113">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="9fc82-113">lastAccessedDateTime</span></span>                  | <span data-ttu-id="9fc82-114">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fc82-114">DateTimeOffset</span></span>        | <span data-ttu-id="9fc82-115">A data e a hora em que o recurso foi acessado pela última vez pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="9fc82-115">The date and time the resource was last accessed by the user.</span></span> <span data-ttu-id="9fc82-116">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="9fc82-116">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9fc82-117">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="9fc82-117">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="9fc82-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9fc82-118">Read-only.</span></span>                      |
| <span data-ttu-id="9fc82-119">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="9fc82-119">lastModifiedDateTime</span></span>              | <span data-ttu-id="9fc82-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9fc82-120">DateTimeOffset</span></span>        | <span data-ttu-id="9fc82-121">A data e a hora em que o recurso foi modificado pela última vez pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="9fc82-121">The date and time the resource was last modified by the user.</span></span> <span data-ttu-id="9fc82-122">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="9fc82-122">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9fc82-123">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="9fc82-123">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="9fc82-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="9fc82-124">Read-only.</span></span>       |
