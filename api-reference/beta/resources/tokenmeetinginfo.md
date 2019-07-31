---
title: tipo de recurso tokenMeetingInfo
description: O tipo tokenMeetingInfo.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 0df9a7a66420f20ff62677f54e617d64e9db0273
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007540"
---
# <a name="tokenmeetinginfo-resource-type"></a><span data-ttu-id="423a4-103">tipo de recurso tokenMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="423a4-103">tokenMeetingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="423a4-104">O tipo tokenMeetingInfo.</span><span class="sxs-lookup"><span data-stu-id="423a4-104">The tokenMeetingInfo type.</span></span>

## <a name="properties"></a><span data-ttu-id="423a4-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="423a4-105">Properties</span></span>

| <span data-ttu-id="423a4-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="423a4-106">Property</span></span>                     | <span data-ttu-id="423a4-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="423a4-107">Type</span></span>    | <span data-ttu-id="423a4-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="423a4-108">Description</span></span>                                                                    |
| :--------------------------- | :------ | :----------------------------------------------------------------------------- |
| <span data-ttu-id="423a4-109">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="423a4-109">allowConversationWithoutHost</span></span> | <span data-ttu-id="423a4-110">Booliano</span><span class="sxs-lookup"><span data-stu-id="423a4-110">Boolean</span></span> | <span data-ttu-id="423a4-111">Indica se uma conversa pode continuar assim que o host da conversa sair.</span><span class="sxs-lookup"><span data-stu-id="423a4-111">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="423a4-112">token</span><span class="sxs-lookup"><span data-stu-id="423a4-112">token</span></span>                        | <span data-ttu-id="423a4-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="423a4-113">String</span></span>  | <span data-ttu-id="423a4-114">O token para ingressar/ativar a reunião.</span><span class="sxs-lookup"><span data-stu-id="423a4-114">The token to join/activate the meeting.</span></span>                                        |

## <a name="json-representation"></a><span data-ttu-id="423a4-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="423a4-115">JSON representation</span></span>

<span data-ttu-id="423a4-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="423a4-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
   "baseType": "microsoft.graph.meetingInfo",
  "@odata.type": "microsoft.graph.tokenMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "token": "String"
}
```

## <a name="example"></a><span data-ttu-id="423a4-117">Exemplo</span><span class="sxs-lookup"><span data-stu-id="423a4-117">Example</span></span>

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
  "suppressions": []
}
-->
