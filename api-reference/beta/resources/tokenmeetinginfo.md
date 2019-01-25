---
title: tipo de recurso de tokenMeetingInfo
description: O tipo de tokenMeetingInfo.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8e115887e67f19375ca8b96a216af98c80e0b312
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513365"
---
# <a name="tokenmeetinginfo-resource-type"></a><span data-ttu-id="cbfc7-103">tipo de recurso de tokenMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="cbfc7-103">tokenMeetingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cbfc7-104">O tipo de tokenMeetingInfo.</span><span class="sxs-lookup"><span data-stu-id="cbfc7-104">The tokenMeetingInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="cbfc7-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cbfc7-105">Properties</span></span>

| <span data-ttu-id="cbfc7-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cbfc7-106">Property</span></span>                     | <span data-ttu-id="cbfc7-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="cbfc7-107">Type</span></span>    | <span data-ttu-id="cbfc7-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="cbfc7-108">Description</span></span>                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| <span data-ttu-id="cbfc7-109">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="cbfc7-109">allowConversationWithoutHost</span></span> | <span data-ttu-id="cbfc7-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="cbfc7-110">Boolean</span></span> | <span data-ttu-id="cbfc7-111">Indica se uma conversa pode continuar depois que deixa o host da conversa.</span><span class="sxs-lookup"><span data-stu-id="cbfc7-111">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="cbfc7-112">token</span><span class="sxs-lookup"><span data-stu-id="cbfc7-112">token</span></span>                        | <span data-ttu-id="cbfc7-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cbfc7-113">String</span></span>  | <span data-ttu-id="cbfc7-114">O token de ingresso/ativar a reunião.</span><span class="sxs-lookup"><span data-stu-id="cbfc7-114">The token to join/activate the meeting.</span></span>                                        |

## <a name="json-representation"></a><span data-ttu-id="cbfc7-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cbfc7-115">JSON representation</span></span>

<span data-ttu-id="cbfc7-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cbfc7-116">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="cbfc7-117">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cbfc7-117">Example</span></span>

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
