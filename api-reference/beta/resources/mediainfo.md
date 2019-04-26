---
title: tipo de recurso mediaInfo
description: As informações de mídia usadas em ações para prompts.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 65cf71f5c116fe213d0e32d560ec24704bff1172
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562592"
---
# <a name="mediainfo-resource-type"></a><span data-ttu-id="3c748-103">tipo de recurso mediaInfo</span><span class="sxs-lookup"><span data-stu-id="3c748-103">mediaInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c748-104">As informações de mídia usadas em ações para prompts.</span><span class="sxs-lookup"><span data-stu-id="3c748-104">The media information used in actions for prompts.</span></span>

## <a name="properties"></a><span data-ttu-id="3c748-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3c748-105">Properties</span></span>
| <span data-ttu-id="3c748-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c748-106">Property</span></span>       | <span data-ttu-id="3c748-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c748-107">Type</span></span>    | <span data-ttu-id="3c748-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c748-108">Description</span></span>                      |
|:---------------|:--------|:---------------------------------|
| <span data-ttu-id="3c748-109">resourceId</span><span class="sxs-lookup"><span data-stu-id="3c748-109">resourceId</span></span>     | <span data-ttu-id="3c748-110">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c748-110">String</span></span>  | <span data-ttu-id="3c748-111">Identidade exclusiva do recurso.</span><span class="sxs-lookup"><span data-stu-id="3c748-111">Unique identity of the resource.</span></span> |
| <span data-ttu-id="3c748-112">URI</span><span class="sxs-lookup"><span data-stu-id="3c748-112">uri</span></span>            | <span data-ttu-id="3c748-113">String</span><span class="sxs-lookup"><span data-stu-id="3c748-113">String</span></span>  | <span data-ttu-id="3c748-114">Caminho para o recurso.</span><span class="sxs-lookup"><span data-stu-id="3c748-114">Path to the resource.</span></span>            |

## <a name="json-representation"></a><span data-ttu-id="3c748-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3c748-115">JSON representation</span></span>

<span data-ttu-id="3c748-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3c748-116">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/mediainfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
