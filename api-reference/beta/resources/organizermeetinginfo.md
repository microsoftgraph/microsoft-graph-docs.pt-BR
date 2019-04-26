---
title: tipo de recurso organizerMeetingInfo
description: Informações de reunião que contêm o organizador da reunião.
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 129e8a60edd89d45eb6e48715a59231475d52b99
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341754"
---
# <a name="organizermeetinginfo-resource-type"></a><span data-ttu-id="d7a76-103">tipo de recurso organizerMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="d7a76-103">organizerMeetingInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d7a76-104">Informações de reunião que contêm o organizador da reunião.</span><span class="sxs-lookup"><span data-stu-id="d7a76-104">Meeting information containing the organizer of the meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="d7a76-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d7a76-105">Properties</span></span>

| <span data-ttu-id="d7a76-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d7a76-106">Property</span></span>                     | <span data-ttu-id="d7a76-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="d7a76-107">Type</span></span>                          | <span data-ttu-id="d7a76-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="d7a76-108">Description</span></span>                                     |
| :--------------------------- | :---------------------------- | :-----------------------------------------------|
| <span data-ttu-id="d7a76-109">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="d7a76-109">allowConversationWithoutHost</span></span> | <span data-ttu-id="d7a76-110">Boolean</span><span class="sxs-lookup"><span data-stu-id="d7a76-110">Boolean</span></span>                       | <span data-ttu-id="d7a76-111">Indica se uma conversa pode continuar assim que o host da conversa sair.</span><span class="sxs-lookup"><span data-stu-id="d7a76-111">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="d7a76-112">organizer</span><span class="sxs-lookup"><span data-stu-id="d7a76-112">organizer</span></span>                    | [<span data-ttu-id="d7a76-113">identitySet</span><span class="sxs-lookup"><span data-stu-id="d7a76-113">identitySet</span></span>](identityset.md) | <span data-ttu-id="d7a76-114">A identidade do Azure Active Directory do organizador.</span><span class="sxs-lookup"><span data-stu-id="d7a76-114">The organizer Azure Active Directory identity.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="d7a76-115">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d7a76-115">JSON representation</span></span>

<span data-ttu-id="d7a76-116">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d7a76-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.meetingInfo",
   "openType": true,
  "@odata.type": "microsoft.graph.organizerMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "organizer": { "@odata.type": "microsoft.graph.identitySet" }
}
```

## <a name="example"></a><span data-ttu-id="d7a76-117">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d7a76-117">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.organizerMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "organizer": {
    "user": {
      "id": "90ED37DC-D8E3-4E11-9DE3-30A955DDA06F",
      "tenantId": "49BFC225-8482-4AB8-94E7-76B48FDB9849"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "organizerMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
