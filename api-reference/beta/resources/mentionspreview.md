---
title: tipo de recurso de mentionsPreview
description: Representa informações sobre objetos mencionam em uma instância de recurso.
localization_priority: Normal
author: simonhult
ms.prod: insights
ms.openlocfilehash: 55eb69d9ef9f6c3686026f6d46a9c78cc4df167b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518762"
---
# <a name="mentionspreview-resource-type"></a><span data-ttu-id="eb024-103">tipo de recurso de mentionsPreview</span><span class="sxs-lookup"><span data-stu-id="eb024-103">mentionsPreview resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb024-104">Representa informações sobre objetos [mencionar](../resources/mention.md) em uma instância de recurso.</span><span class="sxs-lookup"><span data-stu-id="eb024-104">Represents information about [mention](../resources/mention.md) objects in a resource instance.</span></span>

## <a name="properties"></a><span data-ttu-id="eb024-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eb024-105">Properties</span></span>
| <span data-ttu-id="eb024-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb024-106">Property</span></span>     | <span data-ttu-id="eb024-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb024-107">Type</span></span>   |<span data-ttu-id="eb024-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb024-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="eb024-109">isMentioned</span><span class="sxs-lookup"><span data-stu-id="eb024-109">isMentioned</span></span> | <span data-ttu-id="eb024-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb024-110">Boolean</span></span> | <span data-ttu-id="eb024-111">True se o usuário entrou no mencionado na instância do recurso pai.</span><span class="sxs-lookup"><span data-stu-id="eb024-111">True if the signed-in user is mentioned in the parent resource instance.</span></span> <span data-ttu-id="eb024-112">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="eb024-112">Read-only.</span></span> <span data-ttu-id="eb024-113">Oferece suporte a $filter.</span><span class="sxs-lookup"><span data-stu-id="eb024-113">Supports filter.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="eb024-114">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eb024-114">JSON representation</span></span>

<span data-ttu-id="eb024-115">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eb024-115">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.mentionsPreview"
}-->

```json
{
  "isMentioned": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "mentionsPreview resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/mentionspreview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
