---
title: tipo de recurso de tokenMeetingInfo
description: O tipo de tokenMeetingInfo.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8e115887e67f19375ca8b96a216af98c80e0b312
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642587"
---
# <a name="tokenmeetinginfo-resource-type"></a><span data-ttu-id="8c04c-103">tipo de recurso de tokenMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="8c04c-103">tokenMeetingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c04c-104">O tipo de tokenMeetingInfo.</span><span class="sxs-lookup"><span data-stu-id="8c04c-104">The tokenMeetingInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="8c04c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8c04c-105">Properties</span></span>

| <span data-ttu-id="8c04c-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c04c-106">Property</span></span>                     | <span data-ttu-id="8c04c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c04c-107">Type</span></span>    | <span data-ttu-id="8c04c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c04c-108">Description</span></span>                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| <span data-ttu-id="8c04c-109">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="8c04c-109">allowConversationWithoutHost</span></span> | <span data-ttu-id="8c04c-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="8c04c-110">Boolean</span></span> | <span data-ttu-id="8c04c-111">Indica se uma conversa pode continuar depois que deixa o host da conversa.</span><span class="sxs-lookup"><span data-stu-id="8c04c-111">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="8c04c-112">token</span><span class="sxs-lookup"><span data-stu-id="8c04c-112">token</span></span>                        | <span data-ttu-id="8c04c-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8c04c-113">String</span></span>  | <span data-ttu-id="8c04c-114">O token de ingresso/ativar a reunião.</span><span class="sxs-lookup"><span data-stu-id="8c04c-114">The token to join/activate the meeting.</span></span>                                        |

## <a name="json-representation"></a><span data-ttu-id="8c04c-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8c04c-115">JSON representation</span></span>

<span data-ttu-id="8c04c-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8c04c-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "token": "String"
}
```

## <a name="example"></a><span data-ttu-id="8c04c-117">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8c04c-117">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "token": "ABCD123"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "tokenMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/tokenmeetinginfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
