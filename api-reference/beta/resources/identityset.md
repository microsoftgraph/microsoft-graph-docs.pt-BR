---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: IdentitySet
localization_priority: Normal
ms.openlocfilehash: b1570fc0ec0a6e28bab569dfae6992675d8b3537
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333656"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="09c95-102">tipo de recurso identityset</span><span class="sxs-lookup"><span data-stu-id="09c95-102">identitySet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="09c95-103">O \*\*\*\* recurso identityset é uma coleção com chave de recursos de [identidade](identity.md) .</span><span class="sxs-lookup"><span data-stu-id="09c95-103">The **identitySet** resource is a keyed collection of [identity](identity.md) resources.</span></span>

<span data-ttu-id="09c95-104">É usado para representar uma coleção de identidades associada a vários eventos de um item, como _created by_ ou _last modified by_.</span><span class="sxs-lookup"><span data-stu-id="09c95-104">It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="09c95-105">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="09c95-105">JSON representation</span></span>

<span data-ttu-id="09c95-106">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="09c95-106">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identitySet",
  "optionalProperties": [
    "application",
    "applicationInstance",
    "conversation",
    "conversationIdentityType",
    "device",
    "encrypted",
    "guest",
    "phone",
    "user"
  ],
  "openType": true
} -->
```json
{
  "application": {"@odata.type": "microsoft.graph.identity"},
  "applicationInstance": {"@odata.type": "microsoft.graph.identity"},
  "conversation": {"@odata.type": "microsoft.graph.identity"},
  "conversationIdentityType": {"@odata.type": "microsoft.graph.identity"},
  "device": {"@odata.type": "microsoft.graph.identity"},
  "encrypted": {"@odata.type": "microsoft.graph.identity"},
  "guest": {"@odata.type": "microsoft.graph.identity"},
  "phone": {"@odata.type": "microsoft.graph.identity"},
  "user": {"@odata.type": "microsoft.graph.identity"}
}
```

## <a name="properties"></a><span data-ttu-id="09c95-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="09c95-107">Properties</span></span>

| <span data-ttu-id="09c95-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="09c95-108">Property</span></span>    | <span data-ttu-id="09c95-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="09c95-109">Type</span></span>                    | <span data-ttu-id="09c95-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="09c95-110">Description</span></span>                                             |
|:------------|:------------------------|:--------------------------------------------------------|
| <span data-ttu-id="09c95-111">application</span><span class="sxs-lookup"><span data-stu-id="09c95-111">application</span></span> | [<span data-ttu-id="09c95-112">Identidade</span><span class="sxs-lookup"><span data-stu-id="09c95-112">Identity</span></span>](identity.md) | <span data-ttu-id="09c95-p101">Opcional. O aplicativo associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="09c95-p101">Optional. The application associated with this action.</span></span>  |
| <span data-ttu-id="09c95-115">conversation</span><span class="sxs-lookup"><span data-stu-id="09c95-115">conversation</span></span>| [<span data-ttu-id="09c95-116">Identity</span><span class="sxs-lookup"><span data-stu-id="09c95-116">Identity</span></span>](identity.md) | <span data-ttu-id="09c95-117">Opcional.</span><span class="sxs-lookup"><span data-stu-id="09c95-117">Optional.</span></span> <span data-ttu-id="09c95-118">A equipe ou canal associado a esta ação.</span><span class="sxs-lookup"><span data-stu-id="09c95-118">The team or channel associated with this action.</span></span>       |
| <span data-ttu-id="09c95-119">conversationIdentityType</span><span class="sxs-lookup"><span data-stu-id="09c95-119">conversationIdentityType</span></span>| [<span data-ttu-id="09c95-120">Identity</span><span class="sxs-lookup"><span data-stu-id="09c95-120">Identity</span></span>](identity.md) | <span data-ttu-id="09c95-121">Opcional.</span><span class="sxs-lookup"><span data-stu-id="09c95-121">Optional.</span></span> <span data-ttu-id="09c95-122">Indica se a propriedade de **conversa** identifica uma equipe ou um canal.</span><span class="sxs-lookup"><span data-stu-id="09c95-122">Indicates whether the **conversation** property identifies a team or channel.</span></span>|
| <span data-ttu-id="09c95-123">device</span><span class="sxs-lookup"><span data-stu-id="09c95-123">device</span></span>      | [<span data-ttu-id="09c95-124">Identidade</span><span class="sxs-lookup"><span data-stu-id="09c95-124">Identity</span></span>](identity.md) | <span data-ttu-id="09c95-p104">Opcional. O dispositivo associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="09c95-p104">Optional. The device associated with this action.</span></span>       |
| <span data-ttu-id="09c95-127">phone</span><span class="sxs-lookup"><span data-stu-id="09c95-127">phone</span></span>       | [<span data-ttu-id="09c95-128">identity</span><span class="sxs-lookup"><span data-stu-id="09c95-128">identity</span></span>](identity.md) | <span data-ttu-id="09c95-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="09c95-129">Optional.</span></span> <span data-ttu-id="09c95-130">O número de telefone associado a esta ação.</span><span class="sxs-lookup"><span data-stu-id="09c95-130">The phone number associated with this action.</span></span> |
| <span data-ttu-id="09c95-131">user</span><span class="sxs-lookup"><span data-stu-id="09c95-131">user</span></span>        | [<span data-ttu-id="09c95-132">Identity</span><span class="sxs-lookup"><span data-stu-id="09c95-132">Identity</span></span>](identity.md) | <span data-ttu-id="09c95-p106">Opcional. O usuário associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="09c95-p106">Optional. The user associated with this action.</span></span>         |

## <a name="remarks"></a><span data-ttu-id="09c95-135">Comentários</span><span class="sxs-lookup"><span data-stu-id="09c95-135">Remarks</span></span> 

<span data-ttu-id="09c95-136">ConFira [chamada](call.md) para uso \*\*\*\* de recursos identityset.</span><span class="sxs-lookup"><span data-stu-id="09c95-136">See [Call](call.md) for usage of **identitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
