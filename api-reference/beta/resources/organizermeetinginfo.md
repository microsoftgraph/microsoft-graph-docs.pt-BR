---
title: tipo de recurso de organizerMeetingInfo
description: Informações da reunião que contém o organizador da reunião.
author: VinodRavichandran
ms.openlocfilehash: 296b20125908caf73221c2a8380e91931deb7e61
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380209"
---
# <a name="organizermeetinginfo-resource-type"></a><span data-ttu-id="3a87f-103">tipo de recurso de organizerMeetingInfo</span><span class="sxs-lookup"><span data-stu-id="3a87f-103">organizerMeetingInfo resource type</span></span>

> <span data-ttu-id="3a87f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="3a87f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3a87f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3a87f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="3a87f-106">Informações da reunião que contém o organizador da reunião.</span><span class="sxs-lookup"><span data-stu-id="3a87f-106">Meeting information containing the organizer of the meeting.</span></span>

## <a name="properties"></a><span data-ttu-id="3a87f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3a87f-107">Properties</span></span>

| <span data-ttu-id="3a87f-108">Propriedade	</span><span class="sxs-lookup"><span data-stu-id="3a87f-108">Property</span></span>                     | <span data-ttu-id="3a87f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3a87f-109">Type</span></span>                          | <span data-ttu-id="3a87f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3a87f-110">Description</span></span>                                     |
| :--------------------------- | :---------------------------- | :-----------------------------------------------|
| <span data-ttu-id="3a87f-111">allowConversationWithoutHost</span><span class="sxs-lookup"><span data-stu-id="3a87f-111">allowConversationWithoutHost</span></span> | <span data-ttu-id="3a87f-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="3a87f-112">Boolean</span></span>                       | <span data-ttu-id="3a87f-113">Indica se uma conversa pode continuar depois que deixa o host da conversa.</span><span class="sxs-lookup"><span data-stu-id="3a87f-113">Indicates if a conversation can continue once the host of the conversation leaves.</span></span> |
| <span data-ttu-id="3a87f-114">organizer</span><span class="sxs-lookup"><span data-stu-id="3a87f-114">organizer</span></span>                    | [<span data-ttu-id="3a87f-115">identitySet</span><span class="sxs-lookup"><span data-stu-id="3a87f-115">identitySet</span></span>](identityset.md) | <span data-ttu-id="3a87f-116">O organizador da identidade do Windows Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="3a87f-116">The organizer Azure Active Directory identity.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="3a87f-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3a87f-117">JSON representation</span></span>

<span data-ttu-id="3a87f-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3a87f-118">The following is a JSON representation of the resource.</span></span>

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

## <a name="example"></a><span data-ttu-id="3a87f-119">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3a87f-119">Example</span></span>

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
