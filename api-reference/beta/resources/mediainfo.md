---
title: tipo de recurso mediaInfo
description: As informações de mídia usadas em ações para prompts.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 4c6f8e4f4ceea184f9663c433672d0892ed92467
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33342636"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="bdae3-103">tipo de recurso mediaInfo</span><span class="sxs-lookup"><span data-stu-id="bdae3-103">mediaInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdae3-104">As informações de mídia usadas em ações para prompts.</span><span class="sxs-lookup"><span data-stu-id="bdae3-104">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="bdae3-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bdae3-105">Properties</span></span>
| <span data-ttu-id="bdae3-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bdae3-106">Property</span></span>       | <span data-ttu-id="bdae3-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdae3-107">Type</span></span>    | <span data-ttu-id="bdae3-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdae3-108">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="bdae3-109">resourceId</span><span class="sxs-lookup"><span data-stu-id="bdae3-109">resourceId</span></span>     | <span data-ttu-id="bdae3-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bdae3-110">String</span></span>  | <span data-ttu-id="bdae3-111">Identidade exclusiva do recurso.</span><span class="sxs-lookup"><span data-stu-id="bdae3-111">Unique identity of the resource.</span></span> |
| <span data-ttu-id="bdae3-112">URI</span><span class="sxs-lookup"><span data-stu-id="bdae3-112">uri</span></span>            | <span data-ttu-id="bdae3-113">String</span><span class="sxs-lookup"><span data-stu-id="bdae3-113">String</span></span>  | <span data-ttu-id="bdae3-114">Caminho para o recurso.</span><span class="sxs-lookup"><span data-stu-id="bdae3-114">Path to the resource.</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="bdae3-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bdae3-115">JSON representation</span></span>

<span data-ttu-id="bdae3-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bdae3-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mediaInfo"
}-->
```json
{
  "resourceId": "String",
  "uri": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mediaInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
