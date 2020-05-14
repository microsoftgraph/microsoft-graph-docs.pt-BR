---
title: tipo de recurso usageDetails
description: Tipo complexo contendo propriedades de itens usados. Informações sobre quando o recurso foi acessado pela última vez (exibido) ou modificado (editado) pelo usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: d73af15dc3578e9e6c0a568eebfd42480f7065e2
ms.sourcegitcommit: a21fa7fad3a75f94e924b36d6ab94a3699983bdf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/14/2020
ms.locfileid: "44227021"
---
# <a name="usagedetails-resource-type"></a><span data-ttu-id="1ad8d-104">tipo de recurso usageDetails</span><span class="sxs-lookup"><span data-stu-id="1ad8d-104">usageDetails resource type</span></span>

<span data-ttu-id="1ad8d-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ad8d-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1ad8d-106">Tipo complexo contendo propriedades de itens [usados](insights-used.md) .</span><span class="sxs-lookup"><span data-stu-id="1ad8d-106">Complex type containing properties of [Used](insights-used.md) items.</span></span> <span data-ttu-id="1ad8d-107">Informações sobre quando o recurso foi acessado pela última vez (exibido) ou modificado (editado) pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="1ad8d-107">Information on when the resource was last accessed (viewed) or modified (edited) by the user.</span></span>


## <a name="json-representation"></a><span data-ttu-id="1ad8d-108">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1ad8d-108">JSON representation</span></span>

<span data-ttu-id="1ad8d-109">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="1ad8d-109">Here is a JSON representation of the resource</span></span>

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

## <a name="properties"></a><span data-ttu-id="1ad8d-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1ad8d-110">Properties</span></span>

| <span data-ttu-id="1ad8d-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ad8d-111">Property</span></span>              | <span data-ttu-id="1ad8d-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ad8d-112">Type</span></span>          | <span data-ttu-id="1ad8d-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ad8d-113">Description</span></span>  |
| -------------         |---------------| -------------|
| <span data-ttu-id="1ad8d-114">lastAccessedDateTime</span><span class="sxs-lookup"><span data-stu-id="1ad8d-114">lastAccessedDateTime</span></span>                  | <span data-ttu-id="1ad8d-115">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ad8d-115">DateTimeOffset</span></span>        | <span data-ttu-id="1ad8d-116">A data e a hora em que o recurso foi acessado pela última vez pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="1ad8d-116">The date and time the resource was last accessed by the user.</span></span> <span data-ttu-id="1ad8d-117">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="1ad8d-117">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1ad8d-118">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="1ad8d-118">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="1ad8d-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1ad8d-119">Read-only.</span></span>                      |
| <span data-ttu-id="1ad8d-120">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1ad8d-120">lastModifiedDateTime</span></span>              | <span data-ttu-id="1ad8d-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1ad8d-121">DateTimeOffset</span></span>        | <span data-ttu-id="1ad8d-122">A data e a hora em que o recurso foi modificado pela última vez pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="1ad8d-122">The date and time the resource was last modified by the user.</span></span> <span data-ttu-id="1ad8d-123">O carimbo de data/hora representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="1ad8d-123">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="1ad8d-124">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="1ad8d-124">For example, midnight UTC on Jan 1, 2014 would look like this: `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="1ad8d-125">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1ad8d-125">Read-only.</span></span>       |
