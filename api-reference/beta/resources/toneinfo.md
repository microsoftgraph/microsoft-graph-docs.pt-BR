---
title: tipo de recurso de toneInfo
description: Um único evento DTMF.
author: VinodRavichandran
localization_priority: Normal
ms.openlocfilehash: b9be7e0e69be8d127df92f717ab462021f9684b7
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817105"
---
# <a name="toneinfo-resource-type"></a><span data-ttu-id="dbebe-103">tipo de recurso de toneInfo</span><span class="sxs-lookup"><span data-stu-id="dbebe-103">toneInfo resource type</span></span>

> <span data-ttu-id="dbebe-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="dbebe-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="dbebe-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="dbebe-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="dbebe-106">Um único evento DTMF.</span><span class="sxs-lookup"><span data-stu-id="dbebe-106">A single DTMF event.</span></span>

## <a name="properties"></a><span data-ttu-id="dbebe-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dbebe-107">Properties</span></span>

| <span data-ttu-id="dbebe-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dbebe-108">Property</span></span>       | <span data-ttu-id="dbebe-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbebe-109">Type</span></span>    | <span data-ttu-id="dbebe-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbebe-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dbebe-111">sequenceId</span><span class="sxs-lookup"><span data-stu-id="dbebe-111">sequenceId</span></span> | <span data-ttu-id="dbebe-112">Int64</span><span class="sxs-lookup"><span data-stu-id="dbebe-112">Int64</span></span> | <span data-ttu-id="dbebe-113">Um identificador incremental usado para ordenação dos eventos DTMF.</span><span class="sxs-lookup"><span data-stu-id="dbebe-113">An incremental identifier used for ordering DTMF events.</span></span> |
| <span data-ttu-id="dbebe-114">tom</span><span class="sxs-lookup"><span data-stu-id="dbebe-114">tone</span></span> | <span data-ttu-id="dbebe-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbebe-115">String</span></span> | <span data-ttu-id="dbebe-116">Os valores possíveis são: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span><span class="sxs-lookup"><span data-stu-id="dbebe-116">Possible values are: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="dbebe-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dbebe-117">JSON representation</span></span>

<span data-ttu-id="dbebe-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dbebe-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.toneInfo"
}-->
```json
{
  "sequenceId": 1024,
  "tone": "tone0 | tone1 | tone2 | tone3 | tone4 | tone5 | tone6 | tone7 | tone8 | tone9 | star | pound | a | b | c | d | flash"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "toneInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
