---
title: tipo de recurso de toneInfo
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: b4ed9667c2e2156f52703c6fa15f4937ead5cef4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040437"
---
# <a name="toneinfo-resource-type"></a><span data-ttu-id="a1f69-103">tipo de recurso de toneInfo</span><span class="sxs-lookup"><span data-stu-id="a1f69-103">toneInfo resource type</span></span>

> <span data-ttu-id="a1f69-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a1f69-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a1f69-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a1f69-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="a1f69-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a1f69-106">Properties</span></span>

| <span data-ttu-id="a1f69-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a1f69-107">Property</span></span>       | <span data-ttu-id="a1f69-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1f69-108">Type</span></span>    | <span data-ttu-id="a1f69-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1f69-109">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a1f69-110">sequenceId</span><span class="sxs-lookup"><span data-stu-id="a1f69-110">sequenceId</span></span> | <span data-ttu-id="a1f69-111">Int64</span><span class="sxs-lookup"><span data-stu-id="a1f69-111">Int64</span></span> | <span data-ttu-id="a1f69-112">Um identificador incremental usado para ordenação dos eventos DTMF.</span><span class="sxs-lookup"><span data-stu-id="a1f69-112">An incremental identifier used for ordering DTMF events.</span></span> |
| <span data-ttu-id="a1f69-113">tom</span><span class="sxs-lookup"><span data-stu-id="a1f69-113">tone</span></span> | <span data-ttu-id="a1f69-114">String</span><span class="sxs-lookup"><span data-stu-id="a1f69-114">String</span></span> | <span data-ttu-id="a1f69-115">Os valores possíveis são: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span><span class="sxs-lookup"><span data-stu-id="a1f69-115">Possible values are: `tone0`, `tone1`, `tone2`, `tone3`, `tone4`, `tone5`, `tone6`, `tone7`, `tone8`, `tone9`, `star`, `pound`, `a`, `b`, `c`, `d`, `flash`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a1f69-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a1f69-116">JSON representation</span></span>

<span data-ttu-id="a1f69-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a1f69-117">The following is a JSON representation of the resource.</span></span>

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