---
title: tipo de recurso de organizerMeetingInfo
description: Veja a seguir uma representação JSON do recurso.
ms.openlocfilehash: 00a7978c44c82ddd6b34802f29188a554e7e0b4f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037010"
---
# <a name="organizermeetinginfo-resource-type"></a><span data-ttu-id="c34ee-103">tipo de recurso de organizerMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="c34ee-103">organizerMeetingInfo resource type</span></span>

> <span data-ttu-id="c34ee-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c34ee-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c34ee-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c34ee-105">Use of these APIs in production applications is not supported.</span></span>

## <a name="properties"></a><span data-ttu-id="c34ee-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c34ee-106">Properties</span></span>

| <span data-ttu-id="c34ee-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c34ee-107">Property</span></span>                     | <span data-ttu-id="c34ee-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c34ee-108">Type</span></span>                          | <span data-ttu-id="c34ee-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c34ee-109">Description</span></span>                                     |
| :--------------------------- | :---------------------------- | :-----------------------------------------------|
| <span data-ttu-id="c34ee-110">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="c34ee-110">allowConversationWithoutHost</span></span> | <span data-ttu-id="c34ee-111">Booliano</span><span class="sxs-lookup"><span data-stu-id="c34ee-111">Boolean</span></span>                       | <span data-ttu-id="c34ee-112">Indica se uma conversa pode continuar depois que deixa o host da conversa.</span><span class="sxs-lookup"><span data-stu-id="c34ee-112">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="c34ee-113">organizer</span><span class="sxs-lookup"><span data-stu-id="c34ee-113">organizer</span></span>                    | [<span data-ttu-id="c34ee-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="c34ee-114">identitySet</span></span>](identityset.md) | <span data-ttu-id="c34ee-115">O organizador da identidade do Windows Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="c34ee-115">The organizer Azure Active Directory identity.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="c34ee-116">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c34ee-116">JSON representation</span></span>

<span data-ttu-id="c34ee-117">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c34ee-117">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.organizerMeetingInfo"
}-->
```json
{
  "allowConversationWithoutHost": true,
  "organizer": { "@odata.type": "#microsoft.graph.identitySet" }
}
```

## <a name="example"></a><span data-ttu-id="c34ee-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c34ee-118">Example</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "organizerMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
