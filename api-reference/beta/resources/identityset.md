---
author: JeremyKelley
description: O recurso identityset é uma coleção com chave de recursos de identidade.
ms.date: 09/10/2017
title: IdentitySet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: c43981c1f7e79567afe901217030a0b5abed6f53
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006287"
---
# <a name="identityset-resource-type"></a><span data-ttu-id="2be8f-103">tipo de recurso identityset</span><span class="sxs-lookup"><span data-stu-id="2be8f-103">identitySet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2be8f-104">O \*\*\*\* recurso identityset é uma coleção com chave de recursos de [identidade](identity.md) .</span><span class="sxs-lookup"><span data-stu-id="2be8f-104">The **identitySet** resource is a keyed collection of [identity](identity.md) resources.</span></span>

<span data-ttu-id="2be8f-105">É usado para representar uma coleção de identidades associada a vários eventos de um item, como _created by_ ou _last modified by_.</span><span class="sxs-lookup"><span data-stu-id="2be8f-105">It is used to represent a set of identities associated with various events for an item, such as _created by_ or _last modified by_.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2be8f-106">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2be8f-106">JSON representation</span></span>

<span data-ttu-id="2be8f-107">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2be8f-107">The following is a JSON representation of the resource.</span></span>

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

## <a name="properties"></a><span data-ttu-id="2be8f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2be8f-108">Properties</span></span>

| <span data-ttu-id="2be8f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2be8f-109">Property</span></span>    | <span data-ttu-id="2be8f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2be8f-110">Type</span></span>                    | <span data-ttu-id="2be8f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2be8f-111">Description</span></span>                                             |
|:------------|:------------------------|:--------------------------------------------------------|
| <span data-ttu-id="2be8f-112">application</span><span class="sxs-lookup"><span data-stu-id="2be8f-112">application</span></span> | [<span data-ttu-id="2be8f-113">Identidade</span><span class="sxs-lookup"><span data-stu-id="2be8f-113">Identity</span></span>](identity.md) | <span data-ttu-id="2be8f-p101">Opcional. O aplicativo associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="2be8f-p101">Optional. The application associated with this action.</span></span>  |
| <span data-ttu-id="2be8f-116">conversation</span><span class="sxs-lookup"><span data-stu-id="2be8f-116">conversation</span></span>| [<span data-ttu-id="2be8f-117">Identity</span><span class="sxs-lookup"><span data-stu-id="2be8f-117">Identity</span></span>](identity.md) | <span data-ttu-id="2be8f-118">Opcional.</span><span class="sxs-lookup"><span data-stu-id="2be8f-118">Optional.</span></span> <span data-ttu-id="2be8f-119">A equipe ou canal associado a esta ação.</span><span class="sxs-lookup"><span data-stu-id="2be8f-119">The team or channel associated with this action.</span></span>       |
| <span data-ttu-id="2be8f-120">conversationIdentityType</span><span class="sxs-lookup"><span data-stu-id="2be8f-120">conversationIdentityType</span></span>| [<span data-ttu-id="2be8f-121">Identity</span><span class="sxs-lookup"><span data-stu-id="2be8f-121">Identity</span></span>](identity.md) | <span data-ttu-id="2be8f-122">Opcional.</span><span class="sxs-lookup"><span data-stu-id="2be8f-122">Optional.</span></span> <span data-ttu-id="2be8f-123">Indica se a propriedade de **conversa** identifica uma equipe ou um canal.</span><span class="sxs-lookup"><span data-stu-id="2be8f-123">Indicates whether the **conversation** property identifies a team or channel.</span></span>|
| <span data-ttu-id="2be8f-124">device</span><span class="sxs-lookup"><span data-stu-id="2be8f-124">device</span></span>      | [<span data-ttu-id="2be8f-125">Identidade</span><span class="sxs-lookup"><span data-stu-id="2be8f-125">Identity</span></span>](identity.md) | <span data-ttu-id="2be8f-p104">Opcional. O dispositivo associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="2be8f-p104">Optional. The device associated with this action.</span></span>       |
| <span data-ttu-id="2be8f-128">phone</span><span class="sxs-lookup"><span data-stu-id="2be8f-128">phone</span></span>       | [<span data-ttu-id="2be8f-129">identity</span><span class="sxs-lookup"><span data-stu-id="2be8f-129">identity</span></span>](identity.md) | <span data-ttu-id="2be8f-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="2be8f-130">Optional.</span></span> <span data-ttu-id="2be8f-131">O número de telefone associado a esta ação.</span><span class="sxs-lookup"><span data-stu-id="2be8f-131">The phone number associated with this action.</span></span> |
| <span data-ttu-id="2be8f-132">user</span><span class="sxs-lookup"><span data-stu-id="2be8f-132">user</span></span>        | [<span data-ttu-id="2be8f-133">Identity</span><span class="sxs-lookup"><span data-stu-id="2be8f-133">Identity</span></span>](identity.md) | <span data-ttu-id="2be8f-p106">Opcional. O usuário associado a essa ação.</span><span class="sxs-lookup"><span data-stu-id="2be8f-p106">Optional. The user associated with this action.</span></span>         |

## <a name="remarks"></a><span data-ttu-id="2be8f-136">Comentários</span><span class="sxs-lookup"><span data-stu-id="2be8f-136">Remarks</span></span> 

<span data-ttu-id="2be8f-137">Confira [chamada](call.md) para uso \*\*\*\* de recursos identityset.</span><span class="sxs-lookup"><span data-stu-id="2be8f-137">See [Call](call.md) for usage of **identitySet** resources.</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Identity set is a collection of identities",
  "section": "documentation",
  "tocPath": "Resources/IdentitySet"
} -->
